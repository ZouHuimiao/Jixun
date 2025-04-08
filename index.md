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

### 意见反馈
请填写以下表单，您的建议将直接发送至开发者邮箱：

<form id="feedback-form" action="https://formsubmit.co/zouhuimiao0808@icloud.com" method="POST">
  <!-- 隐藏字段配置 -->
  <input type="hidden" name="_captcha" value="false"> <!-- 关闭验证码 -->
  <input type="hidden" name="_subject" value="极训Jixun用户反馈"> <!-- 自定义邮件标题 -->
  <input type="hidden" name="_next" value="https://zouhuimiao.github.io/thank-you.html"> <!-- 提交后跳转页（可选） -->

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

<script>
  const form = document.getElementById('feedback-form');
  form.addEventListener('submit', (e) => {
    e.preventDefault();
    fetch(form.action, {
      method: 'POST',
      body: new FormData(form),
    }).then(() => {
      alert('✅ 提交成功！感谢您的反馈');
      form.reset();
    }).catch(() => {
      alert('❌ 提交失败，请直接邮件联系：zouhuimiao0808@icloud.com');
    });
  });
</script>
