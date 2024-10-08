<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Reflection with PyScript</title>
    <script defer src="https://pyscript.net/latest/pyscript.js"></script>
    <style>
        body {
            font-family: monospace;
            background-color: #829181;
            margin: 0;
            padding: 0;
        }
        .container {
            background-color: #CABFB0;
            margin: 50px auto;
            width: 50%;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        h1 {
            text-align: center;
            color: #829181;
        }
        .content {
            line-height: 1.6;
        }
        .output {
            margin-top: 20px;
        }
    </style>
</head>
<body>

<div class="container">
    <h1>Reflection</h1>
    <div class="content">
        <p id="reflection_text"></p>
        <h3>What I’ve Learned</h3>
        <p id="learned_text"></p>
    </div>
</div>

<py-script>
reflection = """The Data Privacy and Awareness Campaign was an eye-opening event that emphasized how vital it is to protect personal data in the current digital era. 
The growing dependence of humans on technology for diverse parts of their lives has intensified the potential hazards linked to data breaches and abuse. 
This reflection paper aims to investigate the implementation of data privacy principles in technology development and programming by delving into the campaign's main lessons learned."""

learned = """The campaign's emphasis on informed consent was among its most important lessons. People have a right to know how their information is gathered, utilized, and distributed. Programmers need to make sure that their programs have users' express agreement before collecting and processing personal data, hence this concept is especially important in that field.
Another crucial aspect highlighted in the campaign was the importance of data minimization. This principle emphasizes that organizations should only collect and retain the data that is necessary for their purposes. By adhering to data minimization, programmers can reduce the risk of data breaches and ensure that sensitive information is not exposed unnecessarily."""

learned = """ The campaign also emphasized how important data security is. Organizations must employ comprehensive measures to protect personal data against unauthorized access, disclosure, modification, or destruction. This entails carrying out exhaustive risk assessments, upgrading security patches on a regular basis, and encrypting data. To protect user data and uphold confidence, programmers must comprehend and put security best practices into effect.
My awareness and comprehension of data privacy have greatly expanded as a result of the campaign. I'm now more careful about the information I disclose online and the possible repercussions of doing so. In addition, I have strengthened my internet security by utilizing two-factor authentication, creating strong passwords, and being wary of clicking on dubious sites. Furthermore, I've started being pickier about the applications and services I use, taking into account their data practices and privacy policies before giving out personal information.
The Data Privacy and Awareness Campaign has played a pivotal role in increasing consciousness regarding the need of safeguarding personal data. Sensitive information may be protected proactively by individuals and organizations by knowing the concepts of informed consent, data reduction, and data security. It is our duty as programmers to implement these ideas into our work and create apps that put user privacy first.
"""
# Insert text into HTML elements
element_reflection = Element("reflection_text")
element_learned = Element("learned_text")

element_reflection.write(reflection)
element_learned.write(learned)
</py-script>

</body>
</html>
