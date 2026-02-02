<?php
header("Content-Type: text/plain");

$x=$_GET["x"]??null;
$y=$_GET["y"]??null;

if(!ctype_digit($x??"")||!ctype_digit($y??"")||$x==0||$y==0){
  echo "NaN";
  exit;
}

function gcd($a,$b){
  return $b?gcd($b,$a%$b):$a;
}

echo $x/gcd($x,$y)*$y;
