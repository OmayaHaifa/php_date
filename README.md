
	<?php 
		$ok=0;
		echo '<center>';
			echo '<br>'."Today is   ";
			$today = date("y.d.m"); 
			echo $today.'<br>';
			echo "Today is   ";
			$today = date("y/d/m"); 
			echo $today.'<br>';
			echo "Today is   ";
			$today = date("y-d-m"); 
			echo $today.'<br><br>';
		echo "Today is ".date("l").'</br><br>';
	echo"Time is ".date('h:i:s A').'</br><br>';

	if($_POST['day']=='' || $_POST['month']=='' || $_POST['year']=='')
	{
		echo"please enter your birth date to see your age !".'</br>';
		
	}else{
	$myBD = mktime($_POST['month'],$_POST['day'],$_POST['year']);
		echo "My age is ".$myBD." seconds".'</br><br>';
	}
	
		
			echo '<a href="exercice1.html">Retour a la page principale! </a>';
		echo'</center>';
	?>
