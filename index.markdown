---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Parson's Problemen
---
# Parson's Problemen

## Oefening 1
Sorteer de blokken zodat de print opdracht correct wordt uitgevoerd.

<div id="Parsons problem 2-sortableTrash" class="sortable-code"></div> 
<div id="Parsons problem 2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="Parsons problem 2-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="Parsons problem 2-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "naam = input(&quot;Geef jouw naam: &quot;)\n" +
    "eten = input(&quot;Wat is jouw favo eten? &quot; + str(naam) + ”?”)\n" +
    "print(str(eten) + &quot; is een goede keuze!&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "Parsons problem 2-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "trashId": "Parsons problem 2-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#Parsons problem 2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#Parsons problem 2-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>


