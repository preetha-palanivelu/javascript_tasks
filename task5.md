<!-- Task 5
Create textarea to Enter Some sentences below that create a textbox and a button "Search"
now enter some sentence into textarea ..
now if we enter some word into textbox on button click we need to check if that word is present in textarea
For Ex: "Hi my name is Rahul and my city is Pune" this is in textare and in serach textbox we enter "city" on button click we should show alert city exist in textara else City not present -->

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <textarea name="text" id="textplace"></textarea>
  <input type="text" id="textbox" />
  <button id="button" onclick="searchWord()">SEARCH</button>
  <body>
    <script>
      function searchWord() {
        let sentence = document.getElementById("textplace").value;
        let word = document.getElementById("textbox").value;
        let wordFind = sentence.includes(word);
        if (wordFind) {
          alert("The word is found");
        } else {
          alert("The word is not found");
        }
      }
    </script>
  </body>
</html>
