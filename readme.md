# How to modify and implement the calculator script in a web page.

The placeholder script calculates the average Kyte & Doolittle hydrophobicity of a sequence. Odds are that you want to do something else other than that. Here is how to modify the script.

 1. Write CoffeeScript calculations in a file. Save the file as `fasta_calc.coffee`.
   - *In the default CoffeeScript (`fasta_calc.coffee`) the variable `calculation` is used to hold a value to display in the text box. I recommend the easiest thing to do is to just edit what this variable holds.*

 2. Compile CoffeeScript into javascript. Use `coffee -c fasta_calc.coffee`. The file `fasta_calc.js` will appear in the same directory as `fasta_calc.coffee` (unless there are errors in compiling).

 3. Copy contents of `fasta_calc.js` into `index.html` in place of the ellipsis for example:

         <script type = "text/javascript">

             // from textBoxes.html

             function calc(){//paste code below

               //...YOUR SCRIPT HERE

            // stop pasting here!
            } // end calc
        </script>

 4. Open `index.html` in a web browser.

 5. Enter protein sequence into the input box.

 6. Click "*calculate*" and check output.

 Jump to "`<!--HTML layout-->`" in index.html to edit the web server text and style.
