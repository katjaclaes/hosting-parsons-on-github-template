---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Parson's Problemen
---
# Parson's Problemen

## Oefening 1
Sorteer de blokken zodat de print opdracht correct wordt uitgevoerd.

<div id="1-sortableTrash" class="sortable-code"></div> 
<div id="1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="1-feedbackLink" value="Feedback" type="button" /> 
    <input id="1-newInstanceLink" value="Reset" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "naam = input(&quot;Geef jouw naam: &quot;)\n" +
    "eten = input(&quot;Wat is jouw favo eten? &quot; + str(naam) + ”?”)\n" +
    "print(str(eten) + &quot; is een goede keuze!&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "1-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": false,
    "x_indent": 50,
    "lang": "en"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Oefening 2
Zet in de juiste volgorde zodat de totaalprijs wordt afgedrukt.

<div id="2-sortableTrash" class="sortable-code"></div> 
<div id="2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="2-feedbackLink" value="Feedback" type="button" /> 
    <input id="2-newInstanceLink" value="Reset" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "prijs = 3.50\n" +
    "hoeveelheid = 5\n" +
    "totaal = prijs * hoeveelheid\n" +
    "print(totaal)\n";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "2-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": false,
    "x_indent": 50,
    "lang": "en"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#2-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Oefening 3 
Sorteer de blokken zodat ik "A" als resultaat krijg bij een score hoger of gelijk aan 90.

<div id="3-sortableTrash" class="sortable-code"></div> 
<div id="3-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="3-feedbackLink" value="Feedback" type="button" /> 
    <input id="3-newInstanceLink" value="Reset" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "score = int(input(&quot;Wat is je score?&quot;))\n" +
    "if score &gt;= 90:\n" +
    "grade = &quot;A&quot;\n" +
    "else:\n" +
    "grade = &quot;E&quot;\n" +
    "print(grade)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "3-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": false,
    "x_indent": 50,
    "lang": "en"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#3-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#3-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Oefening 4
Vraag twee getallen op en geef weer of getal 1 hoger is dan getal 2:

<div id="4-sortableTrash" class="sortable-code"></div> 
<div id="4-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="4-feedbackLink" value="Feedback" type="button" /> 
    <input id="4-newInstanceLink" value="Reset" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "getal1 = int(input(&quot;Geef een eerste getal: &quot;))\n" +
    "getal2 = int(input(&quot;Geef een tweede getal: &quot;))\n" +
    "if getal1 > getal2: \n" +
    "print(&quot;Getal 1 is groter&quot;)\n";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "4-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": false,
    "x_indent": 50,
    "lang": "en"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#4-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#4-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
