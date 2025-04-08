### **极简、迅速，自我训练，挑战极限**

---

### **应用简介**  
通过极训Jixun，您可以自定义个人知识库进行巩固训练，提升自己，挑战极限。

主要功能和特性如下：
1. 极简的用户界面；
2. 简洁、快速地创建或导入个人知识库；
3. 通过重复训练不断强化和巩固知识点，完善和提升自己；
4. 通过成就系统从各个维度全面评估、掌握和跟踪学习训练进度和状态；
5. 多种知识点展示方式，整合在一个界面，随意组合，简洁高效；
6. 自由度极高地创建和管理课程数据；
7. 分享课程文件，共同学习和进步。

---

### **最新动态**  
- **2025-04-05**：整体框架搭建完成，本地功能首先上线。


---

### **快速导航**  
- [使用条款](terms.md)
- [隐私政策](privacy.md)  
- [常见问题](faq.md)  
- [联系开发者](contact.md)  

---

## 意见反馈
请填写以下表单，您的建议将直接发送至开发者邮箱：

<form id="feedback-form" action="https://formspree.io/f/your-formspree-id" method="POST">
  <div class="form-group">
    <textarea 
      class="feedback-input" 
      name="message" 
      placeholder="请输入您的反馈内容（1000字以内）..." 
      rows="5"
      maxlength="1000"
      required
    ></textarea>
  </div>
  <div class="form-group">
    <input 
      type="email" 
      class="feedback-input" 
      name="email" 
      placeholder="您的邮箱（可选，用于回复）"
    >
  </div>
  <button type="submit" class="feedback-button">提交反馈</button>
</form>

<div id="form-status" class="form-status"></div>

<style>
  .form-group {
    margin-bottom: 1rem;
  }

  .feedback-input {
    width: 100%;
    padding: 12px;
    border: 1px solid #ddd;
    border-radius: 8px;
    font-size: 16px;
    margin: 8px 0;
  }

  .feedback-button {
    background: linear-gradient(135deg, #007BFF, #800080);
    color: white;
    padding: 12px 24px;
    border: none;
    border-radius: 8px;
    cursor: pointer;
    font-size: 16px;
    transition: opacity 0.3s;
  }

  .feedback-button:hover {
    opacity: 0.9;
  }

  .form-status {
    margin-top: 1rem;
    padding: 12px;
    border-radius: 8px;
    display: none;
  }

  .success { background: #e6ffe6; color: #2a752a; }
  .error { background: #ffe6e6; color: #752a2a; }
</style>

<script>
  const form = document.getElementById('feedback-form');
  const statusDiv = document.getElementById('form-status');

  form.addEventListener('submit', async (e) => {
    e.preventDefault();
    
    // 禁用按钮防止重复提交
    const submitBtn = form.querySelector('button[type="submit"]');
    submitBtn.disabled = true;
    submitBtn.textContent = '提交中...';

    try {
      const response = await fetch(form.action, {
        method: 'POST',
        body: new FormData(form),
        headers: { 'Accept': 'application/json' }
      });

      if (response.ok) {
        statusDiv.textContent = '✅ 提交成功！感谢您的反馈';
        statusDiv.className = 'form-status success';
        form.reset();
      } else {
        throw new Error('提交失败');
      }
    } catch (error) {
      statusDiv.textContent = '❌ 提交失败，请直接邮件联系：zouhuimiao0808@icloud.com';
      statusDiv.className = 'form-status error';
    } finally {
      statusDiv.style.display = 'block';
      submitBtn.disabled = false;
      submitBtn.textContent = '提交反馈';
    }
  });
</script>
