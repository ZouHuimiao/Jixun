### **极简、迅速，超越自我，挑战极限**

---

### **应用简介**  
通过极训Jixun，您可以自定义个人知识库进行巩固训练，超越自我，挑战极限。

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
- **2025-04-20**：按题目内容顺序排序，可在题目开头添加序号以控制排序。
- **2025-04-19**：使用github动态更新显示主界面的名言和作者以及仓库中的课程内容。
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

<!-- 在<head>中添加字体和图标 -->
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

<!-- 表单容器 -->
<div class="feedback-container">
  <div class="form-header">
    <h3><i class="fas fa-comment-dots"></i> 意见反馈</h3>
    <p>您的建议将帮助我们做得更好</p>
  </div>

  <form id="feedback-form" action="https://formsubmit.co/zouhuimiao0808@icloud.com" method="POST">
    <!-- 隐藏字段配置 -->
    <input type="hidden" name="_captcha" value="false">
    <input type="hidden" name="_subject" value="极训Jixun用户反馈">
    <input type="hidden" name="_next" value="https://zouhuimiao.github.io/Jixun/thank-you.html">
    <input type="hidden" name="_template" value="table">

    <div class="form-group floating">
      <textarea 
        id="message"
        class="feedback-input" 
        name="message" 
        rows="5"
        maxlength="1000"
        required
      ></textarea>
      <label for="message">请输入您的反馈内容（1000字以内）...</label>
      <div class="char-counter"><span>0</span>/1000</div>
    </div>

    <div class="form-group floating">
      <input 
        id="email"
        type="email" 
        class="feedback-input" 
        name="email"
      >
      <label for="email">您的邮箱（可选，用于回复）</label>
    </div>

    <button type="submit" class="feedback-button">
      <span class="btn-text">提交反馈</span>
      <i class="fas fa-paper-plane"></i>
    </button>
  </form>
</div>

<style>
  /* 基础样式 */
  :root {
    --primary: #6c5ce7;
    --primary-light: #a29bfe;
    --dark: #2d3436;
    --gray: #636e72;
    --light-gray: #dfe6e9;
    --white: #fff;
    --success: #00b894;
  }

  .feedback-container {
    max-width: 600px;
    margin: 2rem auto;
    padding: 2rem;
    background: var(--white);
    border-radius: 16px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
    font-family: 'Inter', sans-serif;
  }

  .form-header {
    text-align: center;
    margin-bottom: 2rem;
  }

  .form-header h3 {
    color: var(--dark);
    font-size: 1.5rem;
    font-weight: 600;
    margin-bottom: 0.5rem;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 0.5rem;
  }

  .form-header p {
    color: var(--gray);
    font-size: 0.9rem;
  }

  /* 浮动标签样式 */
  .floating {
    position: relative;
    margin-bottom: 1.5rem;
  }

  .floating label {
    position: absolute;
    top: 1rem;
    left: 1rem;
    color: var(--gray);
    transition: all 0.3s ease;
    pointer-events: none;
    background: var(--white);
    padding: 0 0.5rem;
  }

  .feedback-input {
    width: 100%;
    padding: 1rem;
    border: 2px solid var(--light-gray);
    border-radius: 8px;
    font-size: 1rem;
    transition: all 0.3s ease;
    background: transparent;
  }

  .feedback-input:focus {
    border-color: var(--primary);
    outline: none;
    box-shadow: 0 0 0 3px rgba(108, 92, 231, 0.2);
  }

  .feedback-input:focus + label,
  .feedback-input:not(:placeholder-shown) + label {
    top: -0.6rem;
    left: 0.8rem;
    font-size: 0.8rem;
    color: var(--primary);
  }

  textarea.feedback-input {
    min-height: 150px;
    resize: vertical;
  }

  /* 字符计数器 */
  .char-counter {
    position: absolute;
    right: 1rem;
    bottom: 1rem;
    font-size: 0.8rem;
    color: var(--gray);
  }

  .char-counter span {
    color: var(--primary);
  }

  /* 按钮样式 */
  .feedback-button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    gap: 0.5rem;
    width: 100%;
    padding: 1rem;
    background: var(--primary);
    color: var(--white);
    border: none;
    border-radius: 8px;
    font-size: 1rem;
    font-weight: 500;
    cursor: pointer;
    transition: all 0.3s ease;
    position: relative;
    overflow: hidden;
  }

  .feedback-button:hover {
    background: var(--primary-light);
    transform: translateY(-2px);
    box-shadow: 0 5px 15px rgba(108, 92, 231, 0.3);
  }

  .feedback-button:active {
    transform: translateY(0);
  }

  .feedback-button i {
    transition: transform 0.3s ease;
  }

  .feedback-button:hover i {
    transform: translateX(5px);
  }

  /* 响应式设计 */
  @media (max-width: 768px) {
    .feedback-container {
      padding: 1.5rem;
      margin: 1rem;
    }
  }
</style>

<script>
  // 字符计数器
  document.getElementById('message').addEventListener('input', function(e) {
    const counter = this.parentElement.querySelector('.char-counter span');
    counter.textContent = this.value.length;
  });

  // 表单提交处理
  document.getElementById('feedback-form').addEventListener('submit', function(e) {
    const btn = this.querySelector('button[type="submit"]');
    btn.disabled = true;
    btn.querySelector('.btn-text').textContent = '提交中...';
    localStorage.setItem('formSubmitted', 'true');
  });

  // 检查是否是从感谢页面返回的
  if(localStorage.getItem('formSubmitted')) {
    const notification = document.createElement('div');
    notification.className = 'form-notification';
    notification.innerHTML = `
      <div class="notification-content">
        <i class="fas fa-check-circle"></i>
        <span>您的反馈已提交成功！</span>
      </div>
    `;
    document.body.appendChild(notification);
    
    setTimeout(() => {
      notification.classList.add('show');
    }, 100);
    
    setTimeout(() => {
      notification.classList.remove('show');
      setTimeout(() => notification.remove(), 300);
    }, 3000);
    
    localStorage.removeItem('formSubmitted');
  }

  // 添加浮动标签的placeholder处理
  document.querySelectorAll('.floating input, .floating textarea').forEach(el => {
    el.setAttribute('placeholder', ' ');
  });
</script>

<style>
  /* 通知样式 */
  .form-notification {
    position: fixed;
    top: 20px;
    right: 20px;
    background: var(--success);
    color: white;
    padding: 1rem 1.5rem;
    border-radius: 8px;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
    transform: translateX(120%);
    transition: transform 0.3s ease;
    z-index: 1000;
  }

  .form-notification.show {
    transform: translateX(0);
  }

  .notification-content {
    display: flex;
    align-items: center;
    gap: 0.5rem;
  }

  .notification-content i {
    font-size: 1.2rem;
  }
</style>
