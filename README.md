# index
The index.html data is provided in the README file


<center><iframe width="560" height="315" src="https://www.youtube.com/embed/PK7p8pcYqls?si=akv0_ws4AD7h63Tf" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe></center>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cloud Computing Quiz</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
        }
        .container {
            width: 60%;
            margin: auto;
            overflow: hidden;
        }
        h1 {
            text-align: center;
            color: #333;
        }
        form {
            background: #fff;
            padding: 20px;
            margin-top: 20px;
            border-radius: 8px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
        }
        .question {
            margin-bottom: 20px;
        }
        .question h3 {
            margin-bottom: 10px;
        }
        .question label {
            display: block;
            margin-bottom: 5px;
        }
        input[type="submit"] {
            background: #5cb85c;
            color: #fff;
            border: none;
            padding: 10px 20px;
            cursor: pointer;
            border-radius: 5px;
            font-size: 16px;
        }
        input[type="submit"]:hover {
            background: #4cae4c;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Cloud Computing Quiz</h1>
        <form id="quizForm">
            <!-- Question 1 -->
            <div class="question">
                <h3>1. What is cloud computing?</h3>
                <label><input type="radio" name="q1" value="a"> A) A type of computing that relies on shared computing resources.</label>
                <label><input type="radio" name="q1" value="b"> B) A method of using wind turbines to power computers.</label>
                <label><input type="radio" name="q1" value="c"> C) A form of computing where you control the weather with software.</label>
            </div>

            <!-- Question 2 -->
            <div class="question">
                <h3>2. Which of the following is a characteristic of cloud computing?</h3>
                <label><input type="radio" name="q2" value="a"> A) Scalability</label>
                <label><input type="radio" name="q2" value="b"> B) Fixed storage capacity</label>
                <label><input type="radio" name="q2" value="c"> C) High latency</label>
            </div>

            <!-- Question 3 -->
            <div class="question">
                <h3>3. What does IaaS stand for in cloud computing?</h3>
                <label><input type="radio" name="q3" value="a"> A) Internet as a Service</label>
                <label><input type="radio" name="q3" value="b"> B) Infrastructure as a Service</label>
                <label><input type="radio" name="q3" value="c"> C) Integration as a Service</label>
            </div>

            <!-- Question 4 -->
            <div class="question">
                <h3>4. Which cloud service model provides the most control over the cloud resources?</h3>
                <label><input type="radio" name="q4" value="a"> A) SaaS (Software as a Service)</label>
                <label><input type="radio" name="q4" value="b"> B) PaaS (Platform as a Service)</label>
                <label><input type="radio" name="q4" value="c"> C) IaaS (Infrastructure as a Service)</label>
            </div>

            <!-- Question 5 -->
            <div class="question">
                <h3>5. Which cloud model is designed for exclusive use by a single organization?</h3>
                <label><input type="radio" name="q5" value="a"> A) Public Cloud</label>
                <label><input type="radio" name="q5" value="b"> B) Private Cloud</label>
                <label><input type="radio" name="q5" value="c"> C) Hybrid Cloud</label>
            </div>

            <!-- Submit Button -->
            <input type="submit" value="Submit Quiz">
        </form>
    </div>

    <script>
        document.getElementById('quizForm').addEventListener('submit', function(event) {
            event.preventDefault();
            let score = 0;
            const correctAnswers = {
                q1: 'a',
                q2: 'a',
                q3: 'b',
                q4: 'c',
                q5: 'b'
            };
            const formData = new FormData(this);
            for (const [question, answer] of formData.entries()) {
                if (answer === correctAnswers[question]) {
                    score++;
                }
            }
            alert('Your Score: ' + score + '/5');
        });
    </script>
</body>
</html>
