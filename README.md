# level-2-task
side hustle level2 task
<?php
/* building a basic voter validation system using php */
$voter_age=12;
$voter_pvc=0;
$voter_ward=02;
/*use if statements to check conditions for a particular voter*/
if ($voter_age>=18 && $voter_pvc==true && $voter_ward==024){
    echo("voter  eligible to vote");
}
elseif ($voter_age>=18 && $voter_pvc==false && $voter_ward==024){
    echo("voter not eligible to vote(no pvc)"); 
}
elseif ($voter_age>=18 && $voter_pvc==true && $voter_ward!==024){
    echo("voter not eligible to vote(invalid ward)");
}
elseif ($voter_age!==18 && $voter_pvc==true && $voter_ward==024){
    echo("voter not eligible to vote(under age voter)");
}
else 
    echo("invalid voter");
?>
