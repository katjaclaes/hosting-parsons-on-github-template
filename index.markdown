---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Parson's Problemen
---
# Parson's Problemen

## Oefening 1
Sorteer de blokken zodat de print opdracht correct wordt uitgevoerd.

<div id="Parsonsproblem2-sortableTrash" class="sortable-code"></div> 
<div id="Parsonsproblem2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="Parsonsproblem2-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="Parsonsproblem2-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "naam = input(&quot;Geef jouw naam: &quot;)\n" +
    "eten = input(&quot;Wat is jouw favo eten? &quot; + str(naam) + ”?”)\n" +
    "print(str(eten) + &quot; is een goede keuze!&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "Parsonsproblem2-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "trashId": "Parsonsproblem2-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#Parsonsproblem2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#Parsonsproblem2-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Oefening 2
Zoek het maximum getal:

<div id="Parsonsproblem5-sortableTrash" class="sortable-code"></div> 
<div id="Parsonsproblem5-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="Parsonsproblem5-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="Parsonsproblem5-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "def find_max(L): \n" +
    "	max = 0\n" +
    "    for item in L:\n" +
    "        if item &gt; max:\n" +
    "            max = item\n" +
    "    return max";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "Parsonsproblem5-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "trashId": "Parsonsproblem5-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#Parsonsproblem5-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#Parsonsproblem5-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Oefening 3 
Sorteer de blokken zodat het totaal bedrag wordt afgedrukt. Let op want niet alle lijnen zijn correct en nodig.

<div id="Parsonsproblem1-sortableTrash" class="sortable-code"></div> 
<div id="Parsonsproblem1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="Parsonsproblem1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="Parsonsproblem1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "prijs = 3.50\n" +
    "hoeveelheid = 5\n" +
    "totaal = prijs * hoeveelheid\n" +
    "print(str(totaal))\n" +
    "print(str(“totaal”)) #distractor\n" +
    "totaal = prijs x hoeveelheid #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "Parsonsproblem1-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "trashId": "Parsonsproblem1-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#Parsonsproblem1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#Parsonsproblem1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Oefening 4
Vraag een nummer op en geef weer of dit even of oneven is:

<div id="Parsonsproblem3-sortableTrash" class="sortable-code"></div> 
<div id="Parsonsproblem3-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="Parsonsproblem3-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="Parsonsproblem3-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "nummer = input(&quot;Geef een nummer: &quot;)\n" +
    "mod = nummer%2\n" +
    "if mod &gt; 0:\n" +
    "   print(&quot;Dit is een oneven nummer!&quot;)\n" +
    "else:\n" +
    "   print(&quot;Dit is een even nummer!&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "Parsonsproblem3-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "trashId": "Parsonsproblem3-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#Parsonsproblem3-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#Parsonsproblem3-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Oefening 5

Maak een gokspel. De computer genereert een willekeurig getal tussen 1 en 9. De gebruiker kan dan het getal raden, de computer geeft vervolgens advies of het hoger of lager moet zijn. De gebruiker kan stoppen door "stop" te typen als gok. De computer schrijft hoeveel keer er gegokt werd wanneer het spel stopt.

<div id="Parsonsproblem4-sortableTrash" class="sortable-code"></div> 
<div id="Parsonsproblem4-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="Parsonsproblem4-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="Parsonsproblem4-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "import random\n" +
    "teller = 1\n" +
    "willekeurigPC = random.randint(1,9)\n" +
    "gok = int(input(&quot;Geef een getal tussen 1 en 9: (Typ stop om te eindigen)&quot;))\n" +
    "while gok != willekeurigPC and gok != &quot;stop&quot;:\n" +
    "    if gok &gt; willekeurigPC:\n" +
    "	    print(&quot;Te hoog&quot;)\n" +
    "    else:\n" +
    "        print(&quot;Te laag&quot;)\n" +
    "    teller = teller + 1\n" +
    "    gok = int(input(&quot;Geef een getal tussen 1 en 9: (Typ stop om te eindigen)&quot;))\n" +
    "print(&quot;Je had &quot; + str(teller) + &quot; gokken nodig!&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "Parsonsproblem4-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "trashId": "Parsonsproblem4-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#Parsonsproblem4-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#Parsonsproblem4-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
