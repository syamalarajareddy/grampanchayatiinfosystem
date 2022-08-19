<?php

include "complaint.php";

$db_hostname='localhost';
$db_username='root';
$db_password='';
$db_name='project';
$db_server = mysqli_connect($db_hostname,$db_username,$db_password,$db_name);
if(!$db_server) die("Unable to connect".mysqli_error());
if( isset($_POST['name']) && isset($_POST['phoneno']) && isset($_POST['email']) && isset($_POST['complaintname']) )
{
	$query="INSERT INTO complaint(name,phoneno,email,complaintname) values('$_POST[name]','$_POST[phoneno]','$_POST[email]','$_POST[complaintname]')";
	$result=mysqli_query($db_server,$query) or die ("query execution error:".mysqli_error($db_server));
	echo "Record entered successfully";
	}
	else
	{
		echo "ERROR: could not able to execute Sql".mysqli_error($db_server);
		}
		
		mysqli_close($db_server);
		
		
?>