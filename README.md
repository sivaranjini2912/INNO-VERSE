<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>INNOVERSE | Paper Presentation</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, Helvetica, sans-serif;
    scroll-behavior:smooth;
}

body{
    background:
        radial-gradient(circle at 15% 20%, rgba(0,255,213,.12), transparent 30%),
        radial-gradient(circle at 85% 80%, rgba(0,140,255,.12), transparent 30%),
        linear-gradient(135deg,#00151f,#003b4d,#001923);
    color:#fff;
    overflow-x:hidden;
}

/* TECH GRID BACKGROUND */
body::before{
    content:"";
    position:fixed;
    inset:0;
    background-image:
        linear-gradient(rgba(0,255,213,.035) 1px,transparent 1px),
        linear-gradient(90deg,rgba(0,255,213,.035) 1px,transparent 1px);
    background-size:45px 45px;
    pointer-events:none;
    z-index:-1;
}

/* COLLEGE HEADER */
header{
    text-align:center;
    padding:30px 15px;
    background:rgba(0,18,28,.85);
    border-bottom:1px solid rgba(0,255,213,.3);
}

.college{
    font-size:clamp(24px,4vw,42px);
    font-weight:900;
    letter-spacing:2px;
}

.college span{
    color:#00ffd5;
}

.subtitle{
    margin-top:8px;
    color:#9deee3;
    font-size:14px;
    letter-spacing:2px;
}

/* MAIN PAPER PRESENTATION */
.hero{
    min-height:82vh;
    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
    padding:60px 20px;
    position:relative;
}

.hero-content{
    max-width:950px;
}

/* SMALL TECH LABEL */
.label{
    display:inline-block;
    padding:10px 22px;
    border:1px solid #00ffd5;
    border-radius:50px;
    color:#00ffd5;
    letter-spacing:3px;
    font-size:13px;
    margin-bottom:25px;
    box-shadow:0 0 20px rgba(0,255,213,.15);
}

/* INNOVERSE */
.hero h1{
    font-size:clamp(55px,12vw,125px);
    font-weight:900;
    letter-spacing:7px;
    background:linear-gradient(
        90deg,
        #00ffd5,
        #00aaff,
        #ffffff,
        #00ffd5
    );
    background-size:300%;
    -webkit-background-clip:text;
    -webkit-text-fill-color:transparent;
    animation:gradient 5s linear infinite;
}

@keyframes gradient{
    from{
        background-position:0%;
    }
    to{
        background-position:300%;
    }
}

/* PAPER PRESENTATION */
.hero h2{
    margin-top:10px;
    font-size:clamp(25px,5vw,48px);
    letter-spacing:2px;
}

.hero p{
    max-width:750px;
    margin:25px auto;
    color:#b8d8df;
    line-height:1.8;
    font-size:17px;
}

/* REGISTER BUTTON */
.register-btn{
    display:inline-block;
    margin-top:15px;
    padding:16px 35px;
    border-radius:40px;
    text-decoration:none;
    color:#001923;
    background:linear-gradient(90deg,#00ffd5,#00aaff);
    font-weight:900;
    letter-spacing:1px;
    box-shadow:0 0 30px rgba(0,255,213,.25);
    transition:.3s;
}

.register-btn:hover{
    transform:translateY(-5px) scale(1.04);
    box-shadow:0 0 45px rgba(0,255,213,.5);
}

/* SCROLL INDICATOR */
.scroll{
    margin-top:50px;
    color:#6caeb8;
    font-size:12px;
    letter-spacing:3px;
    animation:bounce 1.8s infinite;
}

.scroll span{
    display:block;
    margin-top:10px;
    font-size:22px;
    color:#00ffd5;
}

@keyframes bounce{
    0%,100%{
        transform:translateY(0);
    }
    50%{
        transform:translateY(8px);
    }
}

/* COMMON SECTION */
section{
    padding:75px 7%;
}

.title{
    text-align:center;
    font-size:clamp(30px,5vw,48px);
    margin-bottom:45px;
}

.title span{
    color:#00ffd5;
}

/* WHAT IS PAPER PRESENTATION */
.info{
    max-width:1000px;
    margin:auto;
    padding:40px;
    border-radius:25px;
    background:rgba(0,40,55,.65);
    border:1px solid rgba(0,255,213,.2);
    box-shadow:0 0 35px rgba(0,255,213,.08);
}

.info p{
    color:#c7e0e5;
    line-height:2;
    font-size:17px;
    text-align:center;
}

/* DOMAINS */
.domain-grid{
    max-width:1200px;
    margin:auto;
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(230px,1fr));
    gap:22px;
}

.card{
    padding:28px 22px;
    min-height:175px;
    border-radius:20px;
    background:linear-gradient(
        145deg,
        rgba(0,65,80,.8),
        rgba(0,25,40,.8)
    );
    border:1px solid rgba(0,255,213,.18);
    transition:.35s;
    position:relative;
    overflow:hidden;
}

.card::after{
    content:"";
    position:absolute;
    width:100px;
    height:100px;
    right:-35px;
    top:-35px;
    border-radius:50%;
    background:#00ffd5;
    opacity:.08;
}

.card:hover{
    transform:translateY(-8px);
    border-color:#00ffd5;
    box-shadow:0 15px 35px rgba(0,255,213,.15);
}

.number{
    color:#00ffd5;
    font-weight:bold;
    font-size:13px;
    margin-bottom:18px;
}

.card h3{
    font-size:20px;
    line-height:1.4;
}

.card p{
    margin-top:10px;
    color:#86b2bb;
    font-size:14px;
    line-height:1.5;
}

/* RULES */
.rules{
    max-width:1000px;
    margin:auto;
}

.rule{
    display:flex;
    gap:18px;
    padding:20px;
    margin-bottom:15px;
    background:rgba(0,43,58,.7);
    border-left:3px solid #00ffd5;
    border-radius:0 15px 15px 0;
    transition:.3s;
}

.rule:hover{
    transform:translateX(7px);
}

.rule-no{
    min-width:35px;
    height:35px;
    display:flex;
    align-items:center;
    justify-content:center;
    border-radius:50%;
    background:linear-gradient(135deg,#00ffd5,#008cff);
    color:#001923;
    font-weight:bold;
}

.rule p{
    color:#d0e4e8;
    line-height:1.7;
}

/* REGISTRATION */
.registration{
    text-align:center;
}

.registration-box{
    max-width:850px;
    margin:auto;
    padding:45px 25px;
    border-radius:30px;
    background:rgba(0,38,52,.75);
    border:1px solid rgba(0,255,213,.25);
    box-shadow:0 0 40px rgba(0,255,213,.1);
}

.registration-box h3{
    color:#00ffd5;
    font-size:30px;
    margin-bottom:15px;
}

.registration-box p{
    color:#b8d5db;
    line-height:1.8;
    margin-bottom:25px;
}

.big-register{
    display:inline-block;
    padding:17px 40px;
    background:linear-gradient(90deg,#00ffd5,#00aaff);
    color:#001923;
    text-decoration:none;
    border-radius:40px;
    font-weight:900;
    letter-spacing:1px;
    transition:.3s;
}

.big-register:hover{
    transform:scale(1.05);
    box-shadow:0 0 35px rgba(0,255,213,.4);
}

/* FOOTER */
footer{
    text-align:center;
    padding:40px 20px;
    background:#00131c;
    border-top:1px solid rgba(0,255,213,.2);
}

footer h3{
    color:#00ffd5;
    font-size:24px;
    margin-bottom:10px;
}

footer p{
    color:#779da6;
    font-size:14px;
}

/* MOBILE */
@media(max-width:600px){

    .hero{
        min-height:75vh;
        padding:50px 15px;
    }

    .hero h1{
        letter-spacing:3px;
    }

    section{
        padding:60px 5%;
    }

    .info{
        padding:25px 20px;
    }

    .rule{
        padding:16px;
    }

    .registration-box{
        padding:35px 20px;
    }
}
</style>
</head>

<body>

<!-- COLLEGE NAME ONLY -->
<header>
    <div class="college">
        S.A. <span>ENGINEERING COLLEGE</span>
    </div>

    <div class="subtitle">
        DEPARTMENT OF INFORMATION TECHNOLOGY
    </div>
</header>


<!-- PAPER PRESENTATION -->
<section class="hero">

    <div class="hero-content">

        <div class="label">
            PRESENTS
        </div>

        <h1>INNO VERSE</h1>

        <h2>Paper Presentation</h2>

        <p>
            Present your original ideas, explore emerging technologies,
            solve real-world problems and showcase your technical
            creativity and innovation.
        </p>

        <!-- ONLY GOOGLE FORM LINK -->
        <a
            href="https://docs.google.com/forms/d/e/1FAIpQLSdPp41jh0VedVZ5bV3KQ9jC64Theqg233MARSpmRm43diz3ig/viewform?usp=header"
            target="_blank"
            class="register-btn">
            REGISTER NOW →
        </a>

        <div class="scroll">
            SCROLL TO EXPLORE
            <span>↓</span>
        </div>

    </div>

</section>


<!-- WHAT IS PAPER PRESENTATION -->
<section>

    <h2 class="title">
        What is <span>Paper Presentation?</span>
    </h2>

    <div class="info">

        <p>
            A Paper Presentation is a technical platform where participants
            present an original and innovative idea based on a selected
            technology domain. The presentation should explain the problem,
            proposed solution, working approach, technologies involved,
            advantages, applications, expected impact and future scope.
        </p>

    </div>

</section>


<!-- DOMAINS -->
<section>

    <h2 class="title">
        Presentation <span>Domains</span>
    </h2>

    <div class="domain-grid">

        <div class="card">
            <div class="number">01</div>
            <h3>Generative AI</h3>
            <p>
                Intelligent systems and next-generation AI solutions.
            </p>
        </div>

        <div class="card">
            <div class="number">02</div>
            <h3>Cybersecurity</h3>
            <p>
                Security, privacy, threat detection and protection.
            </p>
        </div>

        <div class="card">
            <div class="number">03</div>
            <h3>Quantum Computing</h3>
            <p>
                Quantum technologies and future computational solutions.
            </p>
        </div>

        <div class="card">
            <div class="number">04</div>
            <h3>IoT & Smart Systems</h3>
            <p>
                Connected devices, automation and intelligent systems.
            </p>
        </div>

        <div class="card">
            <div class="number">05</div>
            <h3>Blockchain & Web3</h3>
            <p>
                Decentralization, smart contracts and future web technologies.
            </p>
        </div>

        <div class="card">
            <div class="number">06</div>
            <h3>Digital Twin Technology</h3>
            <p>
                Digital replicas, simulation and intelligent monitoring.
            </p>
        </div>

        <div class="card">
            <div class="number">07</div>
            <h3>AR/VR & Metaverse</h3>
            <p>
                Immersive experiences and extended reality technologies.
            </p>
        </div>

        <div class="card">
            <div class="number">08</div>
            <h3>Green Computing</h3>
            <p>
                Sustainable and energy-efficient computing solutions.
            </p>
        </div>

    </div>

</section>


<!-- RULES -->
<section>

    <h2 class="title">
        Rules & <span>Guidelines</span>
    </h2>

    <div class="rules">

        <div class="rule">
            <div class="rule-no">1</div>
            <p>
                Each team must select only one topic from the given
                themes/domains for the paper presentation.
            </p>
        </div>

        <div class="rule">
            <div class="rule-no">2</div>
            <p>
                Each team can consist of a maximum of 3 members.
            </p>
        </div>

        <div class="rule">
            <div class="rule-no">3</div>
            <p>
                The presentation must be based on an original and innovative
                idea related to the selected theme.
            </p>
        </div>

        <div class="rule">
            <div class="rule-no">4</div>
            <p>
                The presentation should clearly explain Problem Statement,
                Proposed Idea / Solution, Working Principle / Approach,
                Technologies Involved, Advantages and Applications,
                Expected Impact / Future Scope.
            </p>
        </div>

        <div class="rule">
            <div class="rule-no">5</div>
            <p>
                Participants are required to prepare a clear,
                well-structured PPT that effectively represents their idea.
            </p>
        </div>

        <div class="rule">
            <div class="rule-no">6</div>
            <p>
                The presentation should demonstrate creativity,
                innovation, technical understanding, and practical relevance.
            </p>
        </div>

        <div class="rule">
            <div class="rule-no">7</div>
            <p>
                Simply presenting an existing product, application, or
                technology without adding a meaningful new idea,
                improvement, or perspective is not encouraged.
            </p>
        </div>

        <div class="rule">
            <div class="rule-no">8</div>
            <p>
                Each team will be given a maximum of 10 minutes for the
                presentation. Participants should manage their time
                effectively and cover all important aspects within the
                allotted time.
            </p>
        </div>

        <div class="rule">
            <div class="rule-no">9</div>
            <p>
                Participants must be prepared to answer technical and
                conceptual questions from the judges.
            </p>
        </div>

        <div class="rule">
            <div class="rule-no">10</div>
            <p>
                The use of AI tools such as Gamma AI, Claude, ChatGPT, etc.
                to generate the entire PPT or presentation content is
                strongly discouraged. Participants are expected to develop
                and present their own ideas and understanding.
            </p>
        </div>

        <div class="rule">
            <div class="rule-no">11</div>
            <p>
                The presentation should be original and prepared by the
                participants. Any form of plagiarism or direct copying
                from existing sources is discouraged.
            </p>
        </div>

        <div class="rule">
            <div class="rule-no">12</div>
            <p>
                The judges' decision regarding the evaluation and selection
                of winners will be final.
            </p>
        </div>

    </div>

</section>


<!-- REGISTRATION -->
<section id="registration" class="registration">

    <h2 class="title">
        <span>Register</span> for INNOVERSE
    </h2>

    <div class="registration-box">

        <h3>READY TO PRESENT?</h3>

        <p>
            Click the button below to register for the
            INNOVERSE Paper Presentation.
        </p>

        <!-- SAME GOOGLE FORM -->
        <a
            href="https://docs.google.com/forms/d/e/1FAIpQLSdPp41jh0VedVZ5bV3KQ9jC64Theqg233MARSpmRm43diz3ig/viewform?usp=header"
            target="_blank"
            class="big-register">
            OPEN REGISTRATION FORM →
        </a>

    </div>

</section>


<!-- FOOTER -->
<footer>

    <h3>INNOVERSE</h3>

    <p>
        Technical Paper Presentation
    </p>

    <p style="margin-top:8px;">
        S.A. Engineering College (Autonomous)
    </p>

</footer>

</body>
</html>
