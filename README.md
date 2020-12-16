Ghanian culture name is a web application that help people to know their Akan name by entering their date, month and year of birth.                                  Tell display the day they were born and their akan name.
Eric NSHIMIYIMANA Is an author of this web application
In technologies i used to built this web is css, html and javascript.
For those who want to reach me you can terxt me on : nericmpc@gmail.com
I used MIT License
 
 
 
 
 
 
 
 
 
 ANy script in my web application can help you 
 
 <script>
    function check(){
    var mGender = ["Kwasi", "Kwadwo", "Kwabena", "Kwaku", "Yaw", "Kofi", "Kwame"];
    var fGender = ["Akosua", " Adwoa", "Abenaa", "Akua", "Yaa", "Afua", "Ama"];

    var dd = document.getElementById("date").value;
    var mm = document.getElementById("month").value;
    var yr = document.getElementById("year").value;
    var m = document.getElementById("male").selected;
    var f = document.getElementById("female").selected;

    if (document.getElementById("male").selected) {
    var gender = 'male';

    } else {
    var gender = 'female';
    }
    
    //var yr = document.form.year.split(2);
    //var nums = yr.filter(function(elem){
        //document.getElementById("yearmessage").innerHTML="** Your Year **";
        //return !isNaN(elem);
    //});
	if(dd=="")
	{
		alert("Please Enter Your date");
		document.form.date.focus();
		return false;
	}else if(dd <= 0 || dd > 31) {
        alert("Please Enter Valid Date");
		document.form.date.focus();
		return false;
    }
    //if(document.form.date.value <=0 || document.form.date.value >31)
	//{
		//alert("Please Enter Valid Date");
		//document.form.date.focus();
		//return false;
	//}
	else if(mm=="")
	{
		alert("Please Enter your month");
		document.form.month.focus();
		return false;
	}
    else if(mm <=0 || mm >12)
	{
		alert("Please Enter Valid Month");
		document.form.month.focus();
		return false;
	}
	else if(yr=="")
	{
		alert("Please Enter your Year");
		document.form.year.focus();
		return false;
    }
    
    //CALCULATE SECTION YEAR BLOCK
    var yy = yr.slice(0, 2);
    var yy = yr.slice(2, 4);
    var cc = (yy - 1) / 100 + 1;
    var dayOfTheWeek = parseInt(((cc / 4) - 2 * cc - 1) + ((5 * yy / 4)) + ((26 * (mm + 1) / 10)) + dd) % 7;


    if (m) {
    if (dayOfTheWeek == 1) {
    document.getElementById("message").innerHTML =
        alert(" Hello, You were born on Monday and your Akan name is.. " + mGender[1]);
    } else if (dayOfTheWeek == 2) {
    document.getElementById("message").innerHTML =
        alert(" Hello, You were born on Tuesday and your Akan name is.. " + mGender[2]);
    } else if (dayOfTheWeek == 3) {
    document.getElementById("message").innerHTML =
        alert(" Hello, You were born on Wednesday and your Akan name is.. " + mGender[3]);
    } else if (dayOfTheWeek == 4) {
    document.getElementById("message").innerHTML =
        alert(" Hello, You were born on Thursday and your Akan name is.. " + mGender[4]);
    } else if (dayOfTheWeek == 5) {
    document.getElementById("results").innerHTML =
        alert(" Hello, You were born on Friday and your Akan name is.. " + mGender[5]);
    } else if (dayOfTheWeek == 6) {
    document.getElementById("message").innerHTML =
        alert(" Hello, You were born on Saturday and your Akan name is.. " + mGender[6]);
    } else if (dayOfTheWeek == 0) {
    document.getElementById("message").innerHTML =
        alert(" Hello, You were born on Sunday and your Akan name is.. " + maGender[0]);
    }
    }

    //Female Selection Block Function
    else if (f) {
    if (dayOfTheWeek == 1) {
    document.getElementById("message").innerHTML =
        alert(" Hello Dear, You were born on Monday and your Akan name is.. " + fGender[1]);
    } else if (dayOfTheWeek == 2) {
    document.getElementById("message").innerHTML =
        alert(" Hello Dear, You were born on Tuesday and your Akan name is.. " + fGender[2]);
    } else if (dayOfTheWeek == 3) {
    document.getElementById("message").innerHTML =
        alert(" Hello Dear, You were born on Wednesday and your Akan name is.. " + fGender[3]);
    } else if (dayOfTheWeek == 4) {
    document.getElementById("results").innerHTML =
        alert(" Hello Dear, You were born on Thursday and your Akan name is.. " + fGender[4]);
    } else if (dayOfTheWeek == 5) {
    document.getElementById("message").innerHTML =
        alert(" Hello Dear, You were born on Friday and your Akan name is.. " + fGender[5]);
    } else if (dayOfTheWeek == 6) {
    document.getElementById("message").innerHTML =
        alert(" Hello Dear, You were born on Saturday and your Akan name is.. " + fGender[6]);
    } else if (dayOfTheWeek == 0) {
    document.getElementById("message").innerHTML =
        alert(" Hello Dear, You were born on Sunday and your Akan name is.. " + femaleGender[0]);
    }
    }
}
</script>




Setup instructions - includes any scripts that need to be run if necessary.
BDD.

