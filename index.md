<script src="https://cdn.jsdelivr.net/npm/onnxjs/dist/onnx.min.js"></script>
<script src="main.js"></script>

<p  style="font-size:15px;">Input a sequence of zeroes and ones and try to make in random. Neural network will try to predict your                                  next input (it will do it 
                             on the whole sequence at once or after every input - you can change it with "change eval type" button).
                             <br>
                             This model will work only if you are trying to be random, so don't use model predictions when deciding  what to input next. Model corectness level can vary when your sequence is short, but after you input more than ~100 numbers it should be greater than 50% (better than random guessing)
                             <br>
                             Buttons on mobile are slow so don't click too fast.
                             <br>
                             You can use your keyboard to input.
</p>
<br>
<button onclick="change_eval_type()">change eval type</button>    
<br>
<p id="input" style="font-size:20px;"></p>
<br>
<input id="0" type="button" value="0" onclick="zero()" style="width: 49%; height: 200px;">
<input id="1" type="button" value="1" onclick="one()" style="width: 49%; height: 200px;">
<br>
<button id="eval_button" onclick="make_predictions()" style="width: 30%; height: 100px;">Evaluate</button>
<p id="eval" style="font-size:20px;"></p>
<br>
<p id="fast" style="font-size:20px;"></p>
<table id="sequences_table"></table>
