<!-- Task 6
create a textarea Where User will Neter Some Sentence
Create a textbox with placeholder "Replace word" , create 2nd textbox with placeholder "Replace with"
Create a button "Replace"
On Click of Replace - you need to replace word you enter in 1st textbox with word u enter with 2nd textbox in Sentence from textarea and Print that newly Created Sentences into <p> tag -->

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
    <textarea id="sentence"></textarea>
    <input type="text" id="box1" placeholder="Replace word" />
    <input type="text" id="box2" placeholder="Replace with" />
    <button onclick="replace()">REPLACE</button>
    <p></p>
    <script>
      function replace() {
        let sentence = document.getElementById("sentence").value;
        let replaceWord = document.getElementById("box1").value;
        let replaceWith = document.getElementById("box2").value;
        let newSentence = sentence.replace(replaceWord, replaceWith);
        console.log(newSentence);
        document.querySelector("p").innerText = newSentence;
      }
    </script>
  </body>
</html>
