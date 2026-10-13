# invitation
دعوتنامه ایونت افتتاحیه شرکت تجهیزات پزشکی
<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>دعوتنامه پذیرایی</title>
<style>
  :root {
    --green: #2e7d32;
    --green-light: #e8f5e9;
    --green-mid: #4caf50;
    --black: #111;
    --white: #fff;
  }
  * { box-sizing: border-box; margin: 0; padding: 0; }

  body {
    font-family: Tahoma, "Segoe UI", sans-serif;
    background: var(--white);
    color: var(--black);
    line-height: 1.9;
    padding: 20px 14px 60px;
  }

  .card {
    max-width: 720px;
    margin: 0 auto;
    background: var(--white);
    border: 2px solid var(--green);
    border-radius: 18px;
    padding: 30px 24px;
  }

  /* --- سربرگ --- */
  header { text-align: center; margin-bottom: 28px; }
  header h1 {
    color: var(--green);
    font-size: 1.7rem;
    margin-bottom: 10px;
  }
  header p { font-size: 1rem; }

  /* --- بخش‌های فرم --- */
  .step {
    border-top: 1px dashed var(--green-mid);
    padding: 22px 0;
  }
  .step:first-of-type { border-top: none; }

  .step-title {
    display: flex;
    align-items: center;
    gap: 10px;
    font-size: 1.15rem;
    font-weight: bold;
    color: var(--green);
    margin-bottom: 14px;
  }

  /* آیکون‌ها به سبک مینیمال با رنگ سبز */
  .icon {
    width: 30px;
    height: 30px;
    flex: 0 0 30px;
    stroke: var(--green);
    fill: none;
    stroke-width: 1.8;
    stroke-linecap: round;
    stroke-linejoin: round;
  }

  /* --- گزینه‌ها --- */
  .options {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
    gap: 12px;
  }

  label.option {
    display: flex;
    align-items: center;
    gap: 10px;
    border: 2px solid var(--green-mid);
    border-radius: 12px;
    padding: 12px 14px;
    cursor: pointer;
    background: var(--white);
    transition: background .15s, border-color .15s;
    font-size: .98rem;
  }
  label.option:hover { background: var(--green-light); }

  /* وقتی انتخاب شد */
  label.option:has(input:checked) {
    background: var(--green-light);
    border-color: var(--green);
    font-weight: bold;
  }

  input[type="radio"], input[type="checkbox"] {
    accent-color: var(--green);
    width: 18px;
    height: 18px;
  }

  /* --- دکمه ارسال --- */
  .submit-wrap { text-align: center; margin-top: 30px; }

  button {
    background: var(--green);
    color: var(--white);
    border: none;
    border-radius: 12px;
    padding: 14px 40px;
    font-size: 1.05rem;
    font-family: inherit;
    cursor: pointer;
    transition: background .15s;
  }
  button:hover { background: #1b5e20; }

  /* --- پیام تشکر --- */
  #thanks {
    display: none;
    text-align: center;
    color: var(--green);
    margin-top: 26px;
    font-size: 1.1rem;
    font-weight: bold;
  }
</style>
</head>
<body>

<div class="card">

  <header>
    <h1>دعوتنامه‌ی پذیرایی</h1>
    <p>
      سلام و وقت‌بخیر، میهمان عزیز 🌿<br>
      از حضور شما در این مراسم بسیار خوشحالیم و صمیمانه خوش آمد می‌گوییم.
      لطفاً برای آماده‌سازی هرچه بهتر پذیرایی، گزینه‌های موردعلاقه‌ی خود را انتخاب فرمایید.
    </p>
  </header>

  <form id="inviteForm">

    <!-- ۱. ردیف صندلی -->
    <section class="step">
      <div class="step-title">
        <svg class="icon" viewBox="0 0 24 24">
          <rect x="5" y="9" width="14" height="8" rx="2"/>
          <path d="M7 9V6a2 2 0 0 1 2-2h6a2 2 0 0 1 2 2v3"/>
          <path d="M7 17v2M17 17v2"/>
        </svg>
        <span>۱. انتخاب ردیف صندلی</span>
      </div>
      <div class="options">
        <label class="option"><input type="radio" name="row" value="ردیف ۱"> ردیف ۱</label>
        <label class="option"><input type="radio" name="row" value="ردیف ۲"> ردیف ۲</label>
        <label class="option"><input type="radio" name="row" value="ردیف ۳"> ردیف ۳</label>
        <label class="option"><input type="radio" name="row" value="ردیف ۴"> ردیف ۴</label>
        <label class="option"><input type="radio" name="row" value="ردیف ۵"> ردیف ۵</label>
      </div>
    </section>

    <!-- ۲. نوشیدنی -->
    <section class="step">
      <div class="step-title">
        <svg class="icon" viewBox="0 0 24 24">
          <path d="M4 7h13v6a5 5 0 0 1-5 5h-3a5 5 0 0 1-5-5V7z"/>
          <path d="M17 9h2a2 2 0 0 1 0 4h-2"/>
          <path d="M7 3v2M11 3v2M15 3v2"/>
        </svg>
        <span>۲. انتخاب نوشیدنی</span>
      </div>
      <div class="options">
        <label class="option"><input type="radio" name="drink" value="چای"> چای</label>
        <label class="option"><input type="radio" name="drink" value="قهوه"> قهوه</label>
        <label class="option"><input type="radio" name="drink" value="آبمیوه"> آبمیوه</label>
      </div>
    </section>

    <!-- ۳. دسر -->
    <section class="step">
      <div class="step-title">
        <svg class="icon" viewBox="0 0 24 24">
          <path d="M5 11l7-7 7 7z"/>
          <path d="M5 11h14v7a2 2 0 0 1-2 2H7a2 2 0 0 1-2-2v-7z"/>
          <path d="M12 4V2"/>
        </svg>
        <span>۳. انتخاب دسر</span>
      </div>
      <div class="options">
        <label class="option"><input type="radio" name="dessert" value="دسر گرم"> دسر گرم</label>
        <label class="option"><input type="radio" name="dessert" value="دسر سرد"> دسر سرد</label>
      </div>
    </section>

    <!-- ۴. پیش‌غذا -->
    <section class="step">
      <div class="step-title">
        <svg class="icon" viewBox="0 0 24 24">
          <path d="M4 12h16a8 8 0 0 1-8 8 8 8 0 0 1-8-8z"/>
          <path d="M9 8c0-2 1.5-2 1.5-4M14 8c0-2 1.5-2 1.5-4"/>
        </svg>
        <span>۴. انتخاب پیش‌غذا</span>
      </div>
      <div class="options">
        <label class="option"><input type="radio" name="starter" value="سالاد"> سالاد</label>
        <label class="option"><input type="radio" name="starter" value="سوپ"> سوپ</label>
      </div>
    </section>

    <!-- ۵. غذای اصلی -->
    <section class="step">
      <div class="step-title">
        <svg class="icon" viewBox="0 0 24 24">
          <circle cx="12" cy="12" r="8"/>
          <path d="M12 4v16M4 12h16"/>
        </svg>
        <span>۵. انتخاب غذای اصلی</span>
      </div>
      <div class="options">
        <label class="option"><input type="radio" name="main" value="غذای ایرانی سنتی"> ایرانی سنتی</label>
        <label class="option"><input type="radio" name="main" value="فست‌فود"> فست‌فود</label>
      </div>
    </section>

    <!-- ۶. حضور -->
    <section class="step">
      <div class="step-title">
        <svg class="icon" viewBox="0 0 24 24">
          <path d="M20 8v12H4V8"/>
          <path d="M2 8h20v3a2 2 0 0 1-2 2 2 2 0 0 1-2-2 2 2 0 0 1-2 2 2 2 0 0 1-2-2 2 2 0 0 1-2 2 2 2 0 0 1-2-2H4"/>
          <path d="M12 8V5a2 2 0 0 1 4 0"/>
        </svg>
        <span>۶. تمایل به حضور در مراسم</span>
      </div>
      <div class="options">
        <label class="option"><input type="radio" name="attend" value="بله، حضور خواهم داشت" checked> بله، حضور خواهم داشت</label>
        <label class="option"><input type="radio" name="attend" value="متأسفانه نمی‌توانم"> متأسفانه نمی‌توانم</label>
      </div>
    </section>

    <div class="submit-wrap">
      <button type="submit">ثبت انتخاب‌ها</button>
    </div>
  </form>

  <p id="thanks">از همراهی شما سپاسگزاریم 🌿 منتظر حضور گرم شما هستیم.</p>

</div>

<script>
  document.getElementById('inviteForm').addEventListener('submit', function (e) {
    e.preventDefault();
    // اینجا می‌تونید داده‌ها رو به یک سرویس مثل Google Forms / Formspree بفرستید
    const data = new FormData(this);
    const result = {};
    data.forEach((v, k) => result[k] = v);
    console.log('انتخاب‌های میهمان:', result);

    document.getElementById('inviteForm').style.display = 'none';
    document.getElementById('thanks').style.display = 'block';
  });
</script>

</body>
</html>
