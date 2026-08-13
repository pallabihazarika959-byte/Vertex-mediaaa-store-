# Vertex-mediaaa-store-
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1.0">

<title>VERTEX MEDIAAA — Digital Store</title>

<meta name="description"
content="Premium digital books by Vertex Mediaaa — Finance, ambition, mindset and entrepreneurship.">

<style>
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
}

:root{
  --bg:#f5f1e9;
  --paper:#fffdf9;
  --black:#0c0c0c;
  --dark:#151515;
  --gold:#c49a4a;
  --gold2:#e3c47d;
  --text:#171717;
  --muted:#77736b;
  --line:#e5ded2;
  --green:#16a765;
}

html{
  scroll-behavior:smooth;
}

body{
  font-family:Arial,Helvetica,sans-serif;
  background:var(--bg);
  color:var(--text);
  line-height:1.6;
}

a{
  color:inherit;
  text-decoration:none;
}

button{
  font:inherit;
  cursor:pointer;
}

.container{
  max-width:1180px;
  margin:auto;
  padding:0 22px;
}

/* NAV */

nav{
  position:sticky;
  top:0;
  z-index:1000;
  background:rgba(245,241,233,.9);
  backdrop-filter:blur(18px);
  border-bottom:1px solid var(--line);
}

.nav{
  height:76px;
  display:flex;
  align-items:center;
  justify-content:space-between;
}

.logo{
  font-size:20px;
  font-weight:900;
  letter-spacing:2px;
}

.logo span{
  color:var(--gold);
}

.navlinks{
  display:flex;
  gap:28px;
  font-size:14px;
  font-weight:700;
}

.navlinks a:hover{
  color:var(--gold);
}

/* HERO */

.hero{
  min-height:700px;
  display:grid;
  grid-template-columns:1.05fr .95fr;
  align-items:center;
  gap:70px;
}

.badge{
  display:inline-block;
  color:var(--gold);
  font-size:12px;
  font-weight:900;
  letter-spacing:3px;
  text-transform:uppercase;
  margin-bottom:20px;
}

.hero h1{
  font-size:clamp(48px,7vw,88px);
  line-height:.96;
  letter-spacing:-5px;
  margin-bottom:28px;
}

.hero h1 span{
  color:var(--gold);
}

.hero-text{
  max-width:610px;
  color:var(--muted);
  font-size:18px;
  margin-bottom:34px;
}

.buttons{
  display:flex;
  gap:12px;
  flex-wrap:wrap;
}

.btn{
  border:1px solid var(--black);
  padding:14px 23px;
  border-radius:50px;
  font-weight:800;
  display:inline-flex;
  align-items:center;
  justify-content:center;
  transition:.25s;
}

.btn-dark{
  background:var(--black);
  color:#fff;
}

.btn-dark:hover{
  transform:translateY(-3px);
  box-shadow:0 12px 30px #0002;
}

.btn-light{
  background:transparent;
}

.btn-light:hover{
  background:#fff;
}

/* HERO BOOK */

.hero-book{
  display:flex;
  justify-content:center;
}

.book{
  width:310px;
  min-height:440px;
  padding:34px;
  position:relative;
  overflow:hidden;
  border-radius:8px;
  color:white;
  background:
    radial-gradient(circle at 80% 10%,#4c3920 0,transparent 30%),
    linear-gradient(145deg,#252525,#070707);
  box-shadow:25px 35px 70px #0004;
  transform:rotate(2deg);
}

.book:after{
  content:"";
  position:absolute;
  width:280px;
  height:280px;
  border:1px solid #ffffff18;
  border-radius:50%;
  right:-130px;
  top:-100px;
}

.book-brand{
  color:var(--gold2);
  font-size:11px;
  font-weight:900;
  letter-spacing:3px;
}

.book h2{
  margin-top:90px;
  font-size:39px;
  line-height:1;
  letter-spacing:-2px;
}

.book p{
  color:#bbb;
  font-size:13px;
  margin-top:20px;
}

.author{
  position:absolute;
  bottom:30px;
  color:var(--gold2);
  font-size:11px;
  font-weight:bold;
  letter-spacing:2px;
}

/* SECTION */

section{
  padding:95px 0;
}

.dark-section{
  background:#0d0d0d;
  color:white;
}

.section-head{
  max-width:700px;
  margin-bottom:45px;
}

.section-title{
  font-size:clamp(36px,5vw,60px);
  line-height:1;
  letter-spacing:-3px;
  margin-bottom:16px;
}

.section-desc{
  color:var(--muted);
}

.dark-section .section-desc{
  color:#999;
}

/* BOOK CARDS */

.books{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:22px;
}

.book-card{
  background:var(--paper);
  border:1px solid var(--line);
  border-radius:24px;
  padding:28px;
  transition:.25s;
  position:relative;
  overflow:hidden;
}

.book-card:hover{
  transform:translateY(-7px);
  box-shadow:0 25px 60px #0001;
}

.book-number{
  font-size:11px;
  color:var(--gold);
  font-weight:900;
  letter-spacing:2px;
}

.cover{
  height:290px;
  margin:20px 0 25px;
  border-radius:8px;
  display:flex;
  flex-direction:column;
  justify-content:center;
  padding:25px;
  color:white;
  background:
    radial-gradient(circle at 80% 20%,#70582d,transparent 30%),
    linear-gradient(145deg,#252525,#080808);
  box-shadow:0 18px 35px #0002;
}

.cover h3{
  font-size:30px;
  line-height:1;
  letter-spacing:-1.5px;
}

.cover small{
  color:var(--gold2);
  font-weight:900;
  letter-spacing:2px;
  margin-bottom:20px;
}

.book-card h3{
  font-size:25px;
  margin-bottom:8px;
}

.book-card p{
  color:var(--muted);
  font-size:14px;
}

.price{
  font-size:36px;
  font-weight:900;
  margin:22px 0;
}

.buy{
  width:100%;
  border:0;
  padding:15px;
  border-radius:12px;
  background:#111;
  color:#fff;
  font-weight:900;
}

.buy:hover{
  background:#2a2a2a;
}

/* FEATURES */

.features{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:20px;
}

.feature{
  padding:30px;
  border:1px solid #ffffff18;
  border-radius:20px;
  background:#ffffff06;
}

.feature-icon{
  font-size:27px;
  margin-bottom:16px;
}

.feature h3{
  margin-bottom:8px;
}

.feature p{
  color:#999;
  font-size:14px;
}

/* PAYMENT */

.modal{
  position:fixed;
  inset:0;
  z-index:3000;
  background:#000b;
  display:none;
  align-items:center;
  justify-content:center;
  padding:20px;
}

.modal.active{
  display:flex;
}

.modal-box{
  width:100%;
  max-width:470px;
  max-height:92vh;
  overflow:auto;
  background:var(--paper);
  border-radius:25px;
  padding:30px;
  position:relative;
}

.close{
  position:absolute;
  right:18px;
  top:14px;
  border:0;
  background:none;
  font-size:28px;
}

.modal-title{
  font-size:28px;
  font-weight:900;
  margin-bottom:5px;
}

.selected{
  color:var(--muted);
  margin-bottom:20px;
}

.input{
  width:100%;
  border:1px solid var(--line);
  padding:14px;
  border-radius:12px;
  outline:none;
  margin-bottom:12px;
  background:#fff;
}

.input:focus{
  border-color:var(--gold);
}

.pay-box{
  margin:15px 0;
  padding:20px;
  border-radius:18px;
  background:#f3eee5;
  text-align:center;
}

.qr{
  width:210px;
  height:210px;
  margin:15px auto;
  border-radius:14px;
  overflow:hidden;
  background:white;
  padding:7px;
}

.qr img{
  width:100%;
  height:100%;
  object-fit:contain;
}

.upi{
  font-weight:900;
  word-break:break-all;
}

.copy{
  margin-top:10px;
  border:1px solid var(--line);
  padding:9px 15px;
  background:white;
  border-radius:30px;
  font-weight:bold;
}

.pay-options{
  display:grid;
  gap:10px;
}

.whatsapp{
  width:100%;
  padding:15px;
  border:0;
  border-radius:12px;
  background:var(--green);
  color:#fff;
  font-weight:900;
}

.download{
  width:100%;
  padding:15px;
  border:0;
  border-radius:12px;
  background:#111;
  color:#fff;
  font-weight:900;
}

/* FAQ */

.faq{
  max-width:800px;
}

details{
  border-bottom:1px solid var(--line);
  padding:20px 0;
}

summary{
  cursor:pointer;
  font-weight:900;
}

details p{
  color:var(--muted);
  padding-top:12px;
}

/* CONTACT */

.contact{
  text-align:center;
  background:#eae3d7;
}

.contact-links{
  margin-top:25px;
  display:flex;
  justify-content:center;
  flex-wrap:wrap;
  gap:12px;
}

/* FOOTER */

footer{
  background:#090909;
  color:white;
  padding:50px 0;
}

.footer{
  display:flex;
  justify-content:space-between;
  gap:30px;
  flex-wrap:wrap;
}

.footer p{
  color:#888;
  font-size:13px;
}

.footer-logo{
  font-weight:900;
  letter-spacing:2px;
  margin-bottom:7px;
}

.footer-logo span{
  color:var(--gold);
}

/* ADMIN */

.admin{
  margin-top:30px;
  text-align:center;
}

.admin button{
  border:1px solid #333;
  background:#111;
  color:#aaa;
  padding:9px 14px;
  border-radius:30px;
}

/* MOBILE */

@media(max-width:850px){

  .navlinks{
    display:none;
  }

  .hero{
    grid-template-columns:1fr;
    padding-top:65px;
    padding-bottom:70px;
  }

  .hero h1{
    letter-spacing:-3px;
  }

  .hero-book{
    order:-1;
  }

  .books{
    grid-template-columns:1fr;
  }

  .features{
    grid-template-columns:1fr;
  }

  section{
    padding:70px 0;
  }
}

@media(max-width:450px){

  .book{
    width:270px;
    min-height:390px;
  }

  .cover{
    height:250px;
  }

  .hero h1{
    font-size:52px;
  }
}
</style>
</head>

<body>

<!-- NAVBAR -->

<nav>
<div class="container nav">

<a href="#" class="logo">
VERTEX <span>MEDIAAA</span>
</a>

<div class="navlinks">
<a href="#books">Books</a>
<a href="#why">Why Vertex</a>
<a href="#faq">FAQ</a>
<a href="#contact">Contact</a>
</div>

</div>
</nav>


<!-- HERO -->

<header>
<div class="container hero">

<div>

<div class="badge">
VERTEX MEDIAAA STORE
</div>

<h1>
Ideas.<br>
Books.<br>
<span>Influence.</span>
</h1>

<p class="hero-text">
Premium digital books created for ambitious minds.
Learn finance, build yourself, develop your mindset
and turn ideas into action.
</p>

<div class="buttons">

<a href="#books" class="btn btn-dark">
Explore Books
</a>

<a href="#contact" class="btn btn-light">
Contact Us
</a>

</div>

</div>


<div class="hero-book">

<div class="book">

<div class="book-brand">
VERTEX MEDIAAA
</div>

<h2>
DIGITAL<br>
KNOWLEDGE
</h2>

<p>
Read. Learn. Build. Become.
</p>

<div class="author">
NAPUR HAZARIKA
</div>

</div>

</div>

</div>
</header>


<!-- BOOK STORE -->

<section id="books">

<div class="container">

<div class="section-head">

<div class="badge">
THE COLLECTION
</div>

<h2 class="section-title">
Choose your next book.
</h2>

<p class="section-desc">
Three premium digital books. Instant digital access
after your payment is verified.
</p>

</div>


<div class="books">


<!-- BOOK 1 -->

<article class="book-card">

<div class="book-number">
01 / FINANCE
</div>

<div class="cover">

<small>VERTEX MEDIAAA</small>

<h3>
FINANCE<br>
360°
</h3>

</div>

<h3>
Finance 360°
</h3>

<p>
Build a stronger understanding of finance,
money and financial concepts.
</p>

<div class="price">
₹369
</div>

<button
class="buy"
onclick="openPayment(
'Finance 360°',
369,
'finance.pdf'
)">
Buy Finance 360° — ₹369
</button>

</article>


<!-- BOOK 2 -->

<article class="book-card">

<div class="book-number">
02 / AMBITION
</div>

<div class="cover">

<small>VERTEX MEDIAAA</small>

<h3>
VERTEX<br>
OF<br>
AMBITION
</h3>

</div>

<h3>
Vertex of Ambition
</h3>

<p>
A digital book about ambition,
growth and building your future.
</p>

<div class="price">
₹299
</div>

<button
class="buy"
onclick="openPayment(
'Vertex of Ambition',
299,
'vertex-of-ambition.pdf'
)">
Buy Vertex of Ambition — ₹299
</button>

</article>


<!-- BOOK 3 -->

<article class="book-card">

<div class="book-number">
03 / MINDSET
</div>

<div class="cover">

<small>VERTEX MEDIAAA</small>

<h3>
EMPIRE<br>
WITHIN
</h3>

</div>

<h3>
Empire Within
</h3>

<p>
Building the entrepreneur before
the enterprise.
</p>

<div class="price">
₹279
</div>

<button
class="buy"
onclick="openPayment(
'Empire Within',
279,
'empire-within.pdf'
)">
Buy Empire Within — ₹279
</button>

</article>


</div>
</div>
</section>


<!-- WHY VERTEX -->

<section class="dark-section" id="why">

<div class="container">

<div class="section-head">

<div class="badge">
WHY VERTEX
</div>

<h2 class="section-title">
Knowledge designed to move.
</h2>

<p class="section-desc">
Vertex Mediaaa creates practical digital resources
for young people who want to learn, build and grow.
</p>

</div>


<div class="features">

<div class="feature">

<div class="feature-icon">
📚
</div>

<h3>
Premium Books
</h3>

<p>
Carefully structured digital books designed
for practical learning.
</p>

</div>


<div class="feature">

<div class="feature-icon">
⚡
</div>

<h3>
Digital Access
</h3>

<p>
Purchase digitally and receive your selected
book without physical shipping.
</p>

</div>


<div class="feature">

<div class="feature-icon">
🚀
</div>

<h3>
Built for Action
</h3>

<p>
Ideas are valuable when you actually apply them.
</p>

</div>

</div>

</div>
</section>


<!-- FAQ -->

<section id="faq">

<div class="container">

<div class="section-head">

<div class="badge">
FAQ
</div>

<h2 class="section-title">
Questions?
</h2>

</div>


<div class="faq">

<details>

<summary>
How do I purchase a book?
</summary>

<p>
Choose your book, enter your name and email,
then scan the QR code and complete the UPI payment.
</p>

</details>


<details>

<summary>
What payment UPI do you use?
</summary>

<p>
Our UPI ID is 8638490686@fam.
</p>

</details>


<details>

<summary>
What format will I receive?
</summary>

<p>
The books are delivered digitally as PDF files.
</p>

</details>


<details>

<summary>
Can I redistribute the PDF?
</summary>

<p>
No. Purchased books are intended for personal use.
Please do not redistribute or resell the files.
</p>

</details>

</div>

</div>
</section>


<!-- CONTACT -->

<section class="contact" id="contact">

<div class="container">

<div class="badge">
VERTEX MEDIAAA
</div>

<h2 class="section-title">
Let's connect.
</h2>

<p>
For support, collaborations or purchase questions,
contact Vertex Mediaaa.
</p>

<div class="contact-links">

<a
class="btn btn-dark"
href="mailto:napurhazarika26@gmail.com">
📩 Email
</a>

<a
class="btn btn-light"
href="https://instagram.com/znex04"
target="_blank">
📸 Instagram
</a>

<a
class="btn btn-light"
href="https://wa.me/918638490686"
target="_blank">
💬 WhatsApp
</a>

</div>

</div>
</section>


<!-- PAYMENT MODAL -->

<div
class="modal"
id="paymentModal"
onclick="outsideClose(event)">

<div class="modal-box">

<button
class="close"
onclick="closePayment()">
×
</button>

<div class="modal-title">
Complete your order
</div>

<p class="selected" id="selectedBook">
Selected book
</p>


<input
class="input"
id="buyerName"
type="text"
placeholder="Your full name"
autocomplete="name">


<input
class="input"
id="buyerEmail"
type="email"
placeholder="Your email address"
autocomplete="email">


<div class="pay-box">

<strong>
Scan & Pay
</strong>

<div class="qr">

<img
src="qr-cropped.jpg"
alt="Vertex Mediaaa UPI QR Code">
</div>

<div class="upi">
8638490686@fam
</div>

<button
class="copy"
onclick="copyUPI()">
Copy UPI ID
</button>

</div>


<div class="pay-options">

<button
class="whatsapp"
onclick="sendWhatsApp()">
💬 I Have Paid — Send Confirmation
</button>

<button
class="download"
onclick="downloadPDF()">
📥 Download After Verification
</button>

</div>


<p style="
font-size:12px;
color:#888;
margin-top:15px;
text-align:center;
">
Important: downloading is enabled only as a manual
verification workflow in this front-end version.
</p>

</div>
</div>


<!-- FOOTER -->

<footer>

<div class="container footer">

<div>

<div class="footer-logo">
VERTEX <span>MEDIAAA</span>
</div>

<p>
Ideas. Stories. Influence.
</p>

</div>

<div>

<p>
📩 napurhazarika26@gmail.com
</p>

<p>
📸 @znex04
</p>

<p>
© 2026 Vertex Mediaaa. All rights reserved.
</p>

</div>

</div>

</footer>


<script>

/* =========================
   VERTEX MEDIAAA CONFIG
========================= */

const UPI_ID = "8638490686@fam";

const WHATSAPP = "918638490686";

let selectedBook = "";
let selectedPrice = "";
let selectedPDF = "";


/* =========================
   OPEN PAYMENT
========================= */

function openPayment(book,price,pdf){

  selectedBook = book;
  selectedPrice = price;
  selectedPDF = pdf;

  document.getElementById("selectedBook").innerHTML =
    "<strong>" + book + "</strong> — ₹" + price;

  document.getElementById("paymentModal")
    .classList.add("active");

  document.body.style.overflow="hidden";
}


/* =========================
   CLOSE
========================= */

function closePayment(){

  document.getElementById("paymentModal")
    .classList.remove("active");

  document.body.style.overflow="";
}


/* =========================
   OUTSIDE CLICK
========================= */

function outsideClose(event){

  if(event.target.id==="paymentModal"){
    closePayment();
  }

}


/* =========================
   COPY UPI
========================= */

function copyUPI(){

  navigator.clipboard.writeText(UPI_ID)
  .then(()=>{
    alert("UPI ID copied: " + UPI_ID);
  })
  .catch(()=>{
    alert("UPI ID: " + UPI_ID);
  });

}


/* =========================
   WHATSAPP CONFIRMATION
========================= */

function sendWhatsApp(){

  const name =
    document.getElementById("buyerName").value.trim();

  const email =
    document.getElementById("buyerEmail").value.trim();

  if(!name || !email){

    alert("Please enter your name and email first.");

    return;
  }


  const message =
`Hello Vertex Mediaaa 👋

I have purchased:

Book: ${selectedBook}
Amount: ₹${selectedPrice}

Buyer name: ${name}
Buyer email: ${email}

UPI: 8638490686@fam

I have completed the payment.
Please verify my payment and send my PDF.

Thank you.`;

  const url =
    "https://wa.me/" +
    WHATSAPP +
    "?text=" +
    encodeURIComponent(message);

  window.open(url,"_blank");
}


/* =========================
   PDF DOWNLOAD
========================= */

function downloadPDF(){

  const name =
    document.getElementById("buyerName").value.trim();

  const email =
    document.getElementById("buyerEmail").value.trim();

  if(!name || !email){

    alert("Please enter your name and email first.");

    return;
  }


  /*
   IMPORTANT:
   This front-end cannot verify a UPI payment.

   For security, automatic delivery should happen
   only after your payment server confirms payment.

   This button therefore asks for verification first.
  */

  const verified =
    confirm(
      "Only download the PDF if the payment has been verified by Vertex Mediaaa."
    );

  if(!verified) return;

  const link =
    document.createElement("a");

  link.href = selectedPDF;

  link.download = selectedPDF;

  document.body.appendChild(link);

  link.click();

  document.body.removeChild(link);
}

</script>

</body>
</html>
