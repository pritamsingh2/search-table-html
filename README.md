<html>
	<head>
		<title>Search Table</title>
		<meta charset="utf-8">
		<meta name="viewport" content="width=device-width, initial-scale=1">
		<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
		<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
		<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
		<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.6.1/jquery.min.js" type="text/javascript"></script>
		<script src="http://ajax.aspnetcdn.com/ajax/jquery.validate/1.9/jquery.validate.min.js" type="text/javascript"></script>
		<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
		<script src="js/form-validation.js"></script>
	</head>
	<style>
		body{
			border-style:double;
			border-color:black;
			background-color:white;
			border-width: thick;
			border-width: 3px;
		}
		.boxed {
			border: 1px solid black ;
			background-color:lightgrey;
			height: 150px;
			left:10px;
			margin: 3px;
		}
		.tab {
			overflow: hidden;
			background-color: black;
			border-top-left-radius: 5px;
			border-top-right-radius: 5px; 
			border-bottom-left-radius: 5px;
			border-bottom-right-radius: 5px; 
		}
		.tab button {
			background-color: grey;
			float: none;
			border-color:black;
			outline: none;
			cursor: pointer;
			padding: 15px 133px;
			transition: 0.9s;			
		}
		.tab button:hover {
			background-color: #ddd;
		}
		hr{
			border-color:grey;
		}
		#vertical{
			height: 320px;
			border-left: 3px solid black;
			position: absolute;
			top: 5px;
			left: 250px;
			text-align:center;
		}
		.boxed1 {
			border-top: 1px solid black ;
			background-color:lightgrey;
			height: 40px;
			left:5px;
			margin: 10px;
		}
		.previous {
			background-color: black;
			color: white;
			
		}

		.next {
			background-color: black;
			color: white;
		}
		#bar {
			text-decoration: none;
			display: inline-block;
			padding: 5px 10px;
		}
		.panel-primary {
			color: #333;
			background-color: lightgrey;
			border-color:black;
		}
		.nav{
			color: #333;
			background-color: blue;
			border-color:red;
		}
	</style>
	<body>
		<div class="container-fluid">
			<div class="row">
				<div class="panel panel-primary">
					<div class="row">
						<div class="col-sm-12">
							<ul class="nav nav-tabs nav-justified" style="background-color:#8c8c8c;">
								<li><a href="#"><i><b><font color="white" size="3px">All Books</font></b></i></a></li>
								<li><a href="#"><i><b><font color="black" size="3px">Books & E Books</font></b></i></a></li>
								<li><a href="#"><i><b><font color="white" size="3px">Magazine & Journals</font></b></i></a></li>
								<li><a href="#"><i><b><font color="white" size="3px">Media</font></b></i></a></li>
							  </ul>
						</div>
					</div>
					<br>
					<div class="row">
						<div class="col-sm-1">
						</div>
						<div class="col-sm-8">
							<input type="text" name="searchBar" placeholder="Search Content" style="background-color:lightgrey;width:950px;height:30px;border-color:grey;"/>
						</div>
						<div class="col-sm-3">
							<button type="submit" class="searchButton" style="background-color:black;width:150px;height:32px"><font color="white"><b>Search</b></font></button>
						</div>
					</div>
					<br>
					<div  class="row">
						<div class="col-sm-1">
						</div>
						<div class="col-sm-11">
							<u><a href="#">Advanced Search</a></u>
						</div>
					</div>
				</div>
			</div>
			<div class="row">
				<hr>
			</div>
			<div>
				<div class="row">
					<div class="col-sm-2">
						<font color="black" size="3px"><b>Seach result</b></font>
					</div>
				</div>
				<br>
				<div class="row">
					<div class="col-sm-6 text-left">
						<a href="#" ><font color="black">&laquo; Previous </font></a> |
						<a href="#" ><font color="black">Next &raquo;</font></a>
					</div>
					<div class="col-sm-6 text-right">
						<select style="background-color:lightgrey">
							<option value="default">100 Per Page</option>
							<option value="150">150 Per Page</option>
							<option value="200">200 Per Page</option>
							<option value="250">250 Per Page</option>
							<option value="300">300 Per Page</option>

						</select >
						<select style="background-color:lightgrey">
							<option value="default">Sort</option>
							<option value="pageNo">Page wise</option>
							<option value="chapterName">Chapter wise</option>
						</select>
					</div>
				</div>
			</div>
			<div class="row">
				<div class="boxed1">
					<div class="col-sm-2 text-center">
					</div>
					<div class="col-sm-7 text-center">
						<font color="black" size="4px"><b>Description</b></font>
					</div>
					<div class="col-sm-2 text-right">
						<font color="black" size="4px"><b>Select</b></font>
					</div>
				</div>
			</div>
			<div class = "row">
				<div class="col-sm-2 text-center">
					<img src="https://www.nap.edu/cover/12602/450" style="height:60px;width:60px;"/>
				</div>
				<div class="col-sm-7 text-left">
					<font color="black" size="3px"><b>1. Handbook of Agricultural Entomology by Helmut van Emden</b></font><br>
					<font color="black" size="3px"><b>Language: English</b></font><br>
					<font color="black" size="3px"><b>Publisher: New York: [Time-Life Books], [1969-1970]</b></font>
				</div>
				<div class="col-sm-2 text-right">
					<input type="checkbox" id= "checkBox1" style="height:20px;width:20px;">
				</div>
			</div><br>
			<div class = "row">
				<div class="col-sm-2 text-center">
					<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRlhsaGXPBshe1ABMDRQijCFCAwJN75LWGQjxkFYndEIzr53r6E1g"  style="height:60px;width:60px;"></img>
				</div>
				<div class="col-sm-7 text-left">
					<font color="black" size="3px"><b>2. Wild about books by Judy Sierra; Marc Tolon Brown</b></font><br>
					<font color="black" size="3px"><b>Language: English</b></font><br>
					<font color="black" size="3px"><b>Publisher: New York: Alfred A. Knopf, 2004.</b></font>
				</div>
				<div class="col-sm-2 text-right">
					<input type="checkbox" id= "checkBox2"style="height:20px;width:20px;">
				</div>
			</div><br>
			<div class = "row">
				<div class="col-sm-2 text-center">
					<img src="data:image/jpeg;base64,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"  style="height:60px;width:60px;"></img>
				</div>
				<div class="col-sm-7 text-left">
					<font color="black" size="3px"><b>3. The purchase of books by public libraries by Great Britian.</b></font><br>
					<font color="black" size="3px"><b>Language: English</b></font><br>
					<font color="black" size="3px"><b>Publisher: London, H.M. Stationery Off., 1972.</b></font>
				</div>
				<div class="col-sm-2 text-right">
					<input type="checkbox" id= "checkBox3"style="height:20px;width:20px;"><br><br>
					<b><u><a href="#">Read</a>|<a href="#">Download</a></></b>
				</div>
			</div><br>	
			<div class = "row">			
				<div class="col-sm-11 text-right">
					<button type="submit" class="cancelButton" style="background-color:#1a1a1a;width:100px;height:30px"><font color="white"><b>Cancel</b></font></button>
					<button type="submit" class="reserveButton" style="background-color:#1a1a1a;width:100px;height:30px"><font color="white"><b>Reserve</font></button>
				</div>
			</div>
			<div class="row">
				<div class="row">
					<div class="col-sm-2 text-center">
						<font color="black"><b>Speaker Notes</b></font>
					</div>
				</div>
				<br>
				<div class="row">
					<div class="col-sm-2 text-right">					
						<br><a href="#" id="bar" class="previous" data-slide="prev"><font size="5px"> 
							<span class="glyphicon glyphicon-chevron-left"></span></font></a>
					</div>

					<div class="col-sm-2 text-center">
						<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSWaHqVqaM_7SWO3GRv9zx9m9togrZDaT9yEGUDauau-kY9adnr"  style="height:60px;width:60px;"></img>
						<u><font color="black"><b><a href="#">Video Records</a></b></font></u>
					</div>

					<div class="col-sm-3 text-center">
						<img src="https://vignette.wikia.nocookie.net/criminal-case-grimsborough/images/1/1f/Speaker-icon.png/revision/latest?cb=20140611110935"  style="height:60px;width:60px;"></img>
						<u><font color="black"><b><a href="#">Search Audio</a></b></font></u>
					</div>
					
					<div class="col-sm-2 text-center">
						<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSqiOCl_qhZ7z61Psc7b6wktL2UoThPVII3G4X2WQUUN_AZZg-qnA"  style="height:60px;width:60px;"></img>
						<u><font color="black"><b><a href="#">Catagories</a></b></font></u>
					</div>

					<div class="col-sm-2 text-left">
						<br><a href="#" id="bar" class="next" data-slide="next"><font size="5px">
						<span class="glyphicon glyphicon-chevron-right"></span></font></a>
					</div>
				</div>
			</div>
		</div>
	</body>
</html>
