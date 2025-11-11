<!DOCTYPE html>
<html lang="hi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>VISIONARY INSTITUTE OF COMPUTER EDUCATION & CSC CENTER</title>
  <style>
    html, body {
      scroll-behavior: smooth;
      margin: 0;
      padding: 0;
      font-family: "Poppins", Arial, sans-serif;
      background: linear-gradient(to bottom, #e6f0ff, #f8faff);
      overflow-x: hidden;
    }

    header {
      background-color: #004aad;
      color: white;
      text-align: center;
      padding: 20px 0 10px 0;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
    }

    header img {
      height: 110px;
      width: 110px;
      border-radius: 25px;
      border: 4px solid white;
      padding: 5px;
      background: linear-gradient(135deg, #ffffff, #dbe9ff);
      box-shadow: 0 4px 10px rgba(0,0,0,0.3);
      margin-bottom: 5px;
    }

    .vice-text {
      font-size: 26px;
      font-weight: 900;
      background: linear-gradient(90deg, #00b3ff, #0072ff, #004aad);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      letter-spacing: 2px;
      text-transform: uppercase;
      margin: 5px 0;
    }

    header h1 {
      font-size: 22px;
      margin: 8px 0 3px 0;
    }
    header p { margin: 0; font-size: 15px; }

    nav {
      background: #0066cc;
      padding: 10px;
      text-align: center;
      position: sticky;
      top: 0;
      z-index: 100;
    }
    nav a {
      color: white;
      text-decoration: none;
      margin: 0 15px;
      font-weight: bold;
      transition: color 0.3s;
    }
    nav a:hover { color: #ffeb3b; }

    section {
      padding: 20px;
      background: white;
      margin: 20px;
      border-radius: 10px;
      box-shadow: 0 4px 6px rgba(0,0,0,0.1);
      overflow: hidden;
    }

    h2 {
      color: #004aad;
      text-align: center;
      margin-bottom: 15px;
    }
	 h4 {
      color: #F08080;
      text-align: center;
	  font-weight: bold;
      margin-bottom: 15px;
    }

    .service-list {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
      gap: 15px;
      padding: 10px;
    }
    .service-btn {
      display: block;
      background: linear-gradient(90deg, #004aad, #007bff);
      color: white;
      text-decoration: none;
      padding: 12px;
      border-radius: 8px;
      text-align: center;
      font-size: 15px;
      font-weight: bold;
      transition: all 0.3s;
    }
    .service-btn:hover {
      transform: translateY(-3px);
      background: linear-gradient(90deg, #005fe0, #0088ff);
    }

    .gallery {
      display: flex;
      justify-content: center;
      gap: 15px;
      overflow-x: auto;
      padding: 15px 0;
      scroll-behavior: smooth;
    }
    .gallery img {
      height: 200px;
      width: auto;
      max-width: 100%;
      border-radius: 10px;
      flex: 0 0 auto;
      transition: transform 0.3s ease;
      box-shadow: 0 2px 6px rgba(0,0,0,0.2);
    }
    .gallery img:hover { transform: scale(1.05); }

    .btn-whatsapp, .btn-youtube {
      display: inline-block;
      padding: 10px 18px;
      color: white;
      text-decoration: none;
      border-radius: 8px;
      font-weight: bold;
      margin: 5px;
      box-shadow: 0 3px 8px rgba(0,0,0,0.2);
    }
    .btn-whatsapp { background-color: #25D366; }
    .btn-whatsapp:hover { background-color: #1ebe57; }
    .btn-youtube { background-color: #FF0000; }
    .btn-youtube:hover { background-color: #cc0000; }

    form {
      max-width: 450px;
      margin: 25px auto;
      text-align: left;
      background: linear-gradient(145deg, #f8fbff, #e6f0ff);
      border-radius: 15px;
      padding: 25px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
    }
    label {
      font-weight: 600;
      color: #004aad;
      margin-bottom: 5px;
      display: block;
    }
    input, select, textarea {
      width: 100%;
      padding: 10px;
      border: 1px solid #ccc;
      border-radius: 8px;
      margin-bottom: 15px;
      font-size: 14px;
      transition: 0.3s;
    }
    input:focus, select:focus, textarea:focus {
      border-color: #004aad;
      box-shadow: 0 0 5px rgba(0,74,173,0.3);
      outline: none;
    }
    button[type="submit"] {
      width: 100%;
      padding: 12px;
      font-size: 16px;
      font-weight: bold;
      border: none;
      border-radius: 8px;
      background: linear-gradient(90deg, #004aad, #007bff);
      color: white;
      cursor: pointer;
      transition: all 0.3s;
    }
    button[type="submit"]:hover {
      transform: translateY(-2px);
      background: linear-gradient(90deg, #0066ff, #0099ff);
    }

    iframe {
      width: 100%;
      max-width: 600px;
      height: 250px;
      border: 0;
      border-radius: 10px;
    }

    footer {
      text-align: center;
      background: #004aad;
      color: white;
      padding: 10px;
      margin-top: 10px;
      font-size: 14px;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    p {
      text-shadow: 0 0 3px rgba(106, 17, 203, 0.5), 0 0 6px rgba(37, 117, 252, 0.5);
    }

    /* Scrollbar for gallery */
    .gallery::-webkit-scrollbar {
      height: 8px;
    }
    .gallery::-webkit-scrollbar-thumb {
      background: #004aad;
      border-radius: 4px;
    }
	.about-text {
  color: red;
  text-shadow: none; /* glow effect हटाने के लिए */
  text-align: center;
}

  </style>
</head>
<body>

  <header>
    <img src="logo.png" alt="Majid Grahak Sewa Kendra Logo">
    <div class="vice-text">VICE</div>
    <h1>Visionary Institute of Computer Education & CSC Center</h1>
    <p>📍 Fizanagar Basaudhi, Ayodhya</p>
  </header>

  <nav>
    <a href="#home">Home</a>
    <a href="#services">Services</a>
    <a href="#shop">Shop</a>
    <a href="#order">Order</a>
    <a href="#contact">Contact</a>
    <a href="#about">About</a>
  </nav>

  <section id="home">
    <h2>आपका स्वागत है - जहाँ शिक्षा भी, सेवा भी!</h2>
    <p style="text-align:center; font-size:20px; font-weight:500; background: linear-gradient(to right, #6a11cb, #2575fc); -webkit-background-clip: text; -webkit-text-fill-color: transparent; margin: 25px; animation: fadeIn 2s ease-in-out;">
      हमारे Computer Training Center और CSC (जन सेवा केंद्र) में आपका हार्दिक स्वागत है।<br>
      यहाँ Students को मिलता है बेहतरीन कंप्यूटर शिक्षा और Customers को हर सरकारी व गैर-सरकारी सेवा एक ही जगह पर।<br><br>
      Visionary Institute of Computer Education में हम आपका भविष्य संवारने के लिए समर्पित हैं।<br>
      Majid Jansewa Kendra Fizanagar में हम आपकी हर जरूरत को पूरी ईमानदारी और तत्परता से पूरा करते हैं।
    </p>

    <h2 id="services">हमारी ऑनलाइन सेवाएं</h2>
    <div class="service-list">
      <a href="https://uidai.gov.in" target="_blank" class="service-btn">आधार सेवाएं</a>
      <a href="https://www.onlineservices.nsdl.com/paam/endUserRegisterContact.html" target="_blank" class="service-btn">पैन कार्ड सेवा</a>
      <a href="https://passportindia.gov.in" target="_blank" class="service-btn">पासपोर्ट सेवा</a>
      <a href="https://parivahan.gov.in" target="_blank" class="service-btn">ड्राइविंग लाइसेंस सेवा</a>
      <a href="https://nfsa.gov.in" target="_blank" class="service-btn">राशन कार्ड सेवा</a>
      <a href="https://www.csc.gov.in" target="_blank" class="service-btn">CSC लॉगिन पोर्टल</a>
      <a href="https://www.irctc.co.in" target="_blank" class="service-btn">रेलवे टिकट बुकिंग</a>
      <a href="https://www.bharatbillpay.com" target="_blank" class="service-btn">बिजली बिल / मोबाइल रिचार्ज</a>
      <a href="https://www.epfindia.gov.in" target="_blank" class="service-btn">EPF पेंशन सेवा</a>
      <a href="https://eshram.gov.in" target="_blank" class="service-btn">ई-श्रम कार्ड सेवा</a>
      <a href="https://digilocker.gov.in" target="_blank" class="service-btn">डिजिलॉकर सेवा</a>
      <a href="https://www.incometax.gov.in" target="_blank" class="service-btn">इनकम टैक्स पोर्टल</a>
      <a href="https://www.nvsp.in" target="_blank" class="service-btn">NVSP पोर्टल</a>
      <a href="https://upfr.agristack.gov.in/farmer-registry-up/#/" target="_blank" class="service-btn">FARMER REGISTERY पोर्टल</a>
	  
    </div>

   <h4 id="shop">Shop View Inside</h4>
    <div class="gallery">
      <img src="photo1.jpg" alt="shop">
      <img src="photo2.jpg" alt="shop">
      <img src="photo3.jpg" alt="shop">
    </div>

    <!-- SBI CSP Section -->
    <div style="text-align:center; margin:20px 0;">
      <a href="https://wa.me/919936259209?text=मैं%20SBI%20CSP%20से%20संपर्क%20करना%20चाहता%20हूँ" 
         target="_blank" 
         style="display:inline-block; padding:12px 20px; background: linear-gradient(90deg, #004aad, #007bff); color:white; text-decoration:none; font-weight:bold; border-radius:8px; margin-top:10px; box-shadow:0 3px 8px rgba(0,0,0,0.2); transition:all 0.3s;">
        🏦 SBI CSP - खाता खुलवाएँ / जमा / निकासी
      </a>
    </div>

    <h2 id="order">अपना ऑर्डर बुक करें</h2>
    <form id="appointmentForm">
      <label>पूरा नाम:</label>
      <input type="text" id="name" required>
      <label>मोबाइल नंबर:</label>
      <input type="tel" id="phone" pattern="[0-9]{10}" required>
      <label>सेवा चुनें:</label>
      <select id="service" required>
        <option value="">सेवा चुनें</option>
        <option>राशन कार्ड आवेदन</option>
        <option>पैन कार्ड सेवा</option>
        <option>पासपोर्ट सेवा</option>
        <option>ड्राइविंग लाइसेंस आवेदन</option>
        <option>बैंकिंग सेवा</option>
        <option>SBI CSP सेवा (खाता खुलवाएँ / जमा / निकासी)</option>
        <option>मोबाइल रिचार्ज / बिजली बिल भुगतान</option>
        <option>पेंशन / प्रमाण पत्र</option>
        <option>ऑनलाइन फॉर्म भरना</option>
        <option>अन्य सेवा</option>
      </select>
      <label>अपॉइंटमेंट की तारीख:</label>
      <input type="date" id="date" required>
      <label>अतिरिक्त विवरण (यदि कोई हो):</label>
      <textarea id="message" rows="3" placeholder="अपना संदेश लिखें..."></textarea>
      <button type="submit">📅Click here to Send message</button>
    </form>

    <h2 id="contact">संपर्क करें</h2>
    <p style="text-align:center;">📍 Fizanagar Basaudhi, Ayodhya, Uttar Pradesh</p>
    <p style="text-align:center;">📞 9936259209</p>
    <p style="text-align:center;">✉️ mohmajid255@gmail.com</p>
    <center>
      <a href="https://wa.me/919936259209" target="_blank" class="btn-whatsapp">WhatsApp पर संपर्क करें</a>
      <a href="https://www.youtube.com/@StudentofIICE" target="_blank" class="btn-youtube">🎥 YouTube चैनल देखें</a>
    </center><br>

    <center>
      <iframe 
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d4420.3155021946395!2d81.6170178761184!3d26.76903396624911!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x399a2fff4430bc07%3A0xe01b1c288228b9d5!2sParag%20Doodh%20Dairy!5e1!3m2!1sen!2sin!4v1762839813704!5m2!1sen!2sin"
        allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade">
      </iframe>
    </center>
	
    <h2 id="about">हमारे बारे में</h2>
<p class="about-text">
Majid Grahak Sewa Kendra, अयोध्या में स्थित एक भरोसेमंद और प्रतिष्ठित केंद्र है। हमारे यहाँ ग्राहकों को सरकारी और गैर-सरकारी सभी सेवाएँ एक ही स्थान पर उपलब्ध हैं, जैसे कि आधार कार्ड सेवा, पैन कार्ड सेवा, पासपोर्ट आवेदन, ड्राइविंग लाइसेंस आवेदन, राशन कार्ड सेवा, बैंकिंग सेवाएँ और SBI CSP (खाता खुलवाना, जमा / निकासी), मोबाइल रिचार्ज और बिजली बिल भुगतान, EPF पेंशन सेवा, ई-श्रम कार्ड और डिजिलॉकर सेवाएँ, तथा अन्य सभी ऑनलाइन सरकारी फॉर्म भरना।

साथ ही हम बच्चों और युवाओं के लिए Computer Coaching Classes भी संचालित करते हैं, जिसमें उन्हें बेसिक से एडवांस तक कंप्यूटर शिक्षा प्रदान की जाती है, ताकि वे अपने भविष्य के लिए तैयार हो सकें।

हमारा उद्देश्य है कि हर ग्राहक और छात्र को सुविधाजनक, भरोसेमंद और पारदर्शी सेवा मिले। यहाँ शिक्षा भी है, सेवा भी, और आपका विश्वास हमारा सर्वोच्च लक्ष्य है।
</p>
  </section>

  <footer>
    <p>📞 9936259209 | © 2025 Visionary Institute of Computer Education & CSC Center</p>
  </footer>

  <script>
    document.getElementById("appointmentForm").addEventListener("submit", function(e){
      e.preventDefault();
      let name = document.getElementById("name").value;
      let phone = document.getElementById("phone").value;
      let service = document.getElementById("service").value;
      let date = document.getElementById("date").value;
      let message = document.getElementById("message").value;

      let whatsappMessage = `📝 *नया अपॉइंटमेंट बुकिंग विवरण*%0A👤 नाम: ${name}%0A📞 मोबाइल: ${phone}%0A🛠 सेवा: ${service}%0A📅 तारीख: ${date}%0A💬 संदेश: ${message}`;
      let whatsappURL = `https://wa.me/919936259209?text=${whatsappMessage}`;
      window.open(whatsappURL, "_blank");
    });
  </script>

</body>
</html>
