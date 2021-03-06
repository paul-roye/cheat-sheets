# Main metrics

<ul>
<li class="limetrics"> <span class="concept">Quality Gate Status</span> : State of the quality gate associated to the project. Possible values: ERROR, WARN, OK. It changes after each scan. </li>
<li class="limetrics"> <span class="concept">Reliability</span> : Number of bugs, number of new bugs, etc... Reliability rating: A = 0 bug, B = at least **1 Minor** bug,
   C = at least 1 **Major** bug, D = at least **1 critical** bug, E = at least **1 Blocker** bug</li>
<li class="limetrics"> <span class="concept">Security</span> : Number of vulnerabilities, number of new vulnerabilities, etc... Reliability rating same as Reliability rating</li>
<li class="limetrics"> <span class="concept">Complexity</span> Cyclomatic complexity is used up to version 6.3. 
It's measured on choices and branches i.e. numbers of if, else, while, switch/case
It is recommended to have at least a cyclomatic complexity of 12 in a method. Each method add 1 to the complexity.</li>
</ul>
```
String getMonth (int monthNumber) {//+1
   switch (monthNumber) {
    case 1:                        //+1
       return "January";
    case 2:                       //+1
       return "February";
    default:
    return "Error";
  }
}
``` 
<ul>
<li class="limetrics"> <span class="concept">Metric</span> : Number of classes, files, lines, lines of code,methods, projects, statements ....</li>
<li class="limetrics"> <span class="concept">Duplications</span> : duplicated blocks, files, lines</li>
<li class="limetrics"> <span class="concept">Maintainability</span> : Number of code smells, technical debt i.e effort to fix all maintainability issues.</li>
<li class="limetrics"> <span class="concept">Tests</span> : Condition coverage, line coverage, etc...</li>
</ul>

```
Condition coverage = (conditions evaluated to true at least once + conditions evaluated to false at least once ) / (2* total number of conditions)
boolean a = false;
boolean b = true;
boolean c = false;

if(a && (b || c) ){ ...}

Condition coverage =  (2 + 1) / (2*3) = 0.5 
``` 
