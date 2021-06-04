<script>
function setNameData(){
		let element = document.getElementById('nameField');
		document.cookie = "data="+element.value;
		let btn1 = document.getElementById('saveBtn');
		document.getElementById('nameCookie').innerHTML=element.value;
	}

	function setBrowser(){
		let element = document.getElementById('browserField');
		document.cookie = "data="+element.value;
		let btn2 = document.getElementById('saveBtn2');
		document.getElementById('browserCookie').innerHTML=element.value;
	}

	var OSName = "Unknown";
	if (window.navigator.userAgent.indexOf("Windows NT 10.0")!= -1) OSName="Windows 10";
	if (window.navigator.userAgent.indexOf("Windows NT 6.2") != -1) OSName="Windows 8";
	if (window.navigator.userAgent.indexOf("Windows NT 6.1") != -1) OSName="Windows 7";
	if (window.navigator.userAgent.indexOf("Mac")            != -1) OSName="Mac/iOS";
	if (window.navigator.userAgent.indexOf("X11")            != -1) OSName="UNIX";
	if (window.navigator.userAgent.indexOf("Linux")          != -1) OSName="Linux";
	document.cookie = "operating-system="+OSName;
	document.getElementById('detectOS').innerHTML=OSName;
</script>

<body>
<input id="nameField" type="text" class="form-control " placeholder="Nume si Prenume">
<button class="btn btn-success custom" type="button" id="saveBtn" onclick="setNameData()">Save</button>
<br>

<input id="browserField" type="text" class="form-control " placeholder="Browser">
<button class="btn btn-success custom" type="button" id="saveBtn2" onclick="setBrowser()">Save</button>
<br><br>

Nume si Prenume: <b><span id="nameCookie"></span></b><br>
Browser:<b><span id="browserCookie"></span></b><br>
OS:<b><span id="detectOS"></span></b><br>

<hr>
<div style="text-align:center; font-family:'Arial Black';"> Notă de informare privind prelucrarea datelor cu caracter personal </div>
<br>
În conformitate cu prevederile Regulamentului (UE) 2016/679 privind protecția persoanelor fizice în ceea ce privește prelucrarea datelor cu caracter personal și privind libera circulație a acestor date Universitatea Tehnică din Cluj Napoca, Masterul de eActivități  prelucrează în condiții de siguranță datele personale furnizate.
 Vă notificăm faptul că datorită temeiului legal aplicabil în România și a relației contractuale în care vă aflați cu Universitatea Tehnică din Cluj-Napoca, Masterul de eActivități și stagiul de mobilitate Erasmus în UK, aceasta procesează pe perioada relațiilor contractuale următoarele categorii de informații personale care vă aparțin pe care le deține la nivelul departamentelor și serviciilor: date de identificare conform actelor personale emise de autoritățile statului român (certificat de naștere, carte de identitate, pașaport unde e cazul, etc.); date financiare (număr de cont, venituri realizate la nivelul instituției, situații financiare personale, etc.); caracteristici personale (vârsta, locul nașterii, naționalitate, stare civilă, etc. necesare pentru stabilirea de drepturi cuvenite); opinii privind starea de sănătate (în baza certificatelor și adeverințelor medicale și de evaluare a stării de sănătate stipulate în normativele aplicabile); componența familiei (numărul de copii și date de identificare a acestora, stare civilă, etc. in baza cărora se fac justificările de calcul a unor drepturi cuvenite sau se stabilesc alte drepturi conform legilor și normativelor aplicabile pentru cei care optează sau solicită aceste drepturi); informații privind parcursul academic, calificările deținute, istoricul profesional, calitatea de membru in organizații profesionale, publicații, date de contact necesare pentru derularea curentă a activității educaționale și de cercetare specifice universității.
Menționăm ca reținerea datelor cu caracter personal în instituție are rolul de a putea furniza către titularul datelor, la cerere, informații privind perioada de școlarizare petrecută în cadrul instituției și după finalizarea acestei perioade de instruire și se supune suplimentar temeiului legal aplicabil în România furnizat de OM Nr. 657 / 24.11.2014 privind regimul actelor de studii în sistemul de învățământ superior cu completările ulterioare.
Datele sunt prelucrate în scopul încheierii și executării contractelor și raporturilor juridice specifice stagiului de mobilitate Erasmus în UK, pentru activitățile necesare în vederea îndeplinirii scopului pentru care universitatea a fost creată - educație și cultură, fiind folosite și pentru analize, prelucrări statistice și arhivare, conform prevederilor legale.
La nivel național respectarea drepturilor persoanelor cu privire la datele cu caracter personal este monitorizată de Autoritatea Națională de Supraveghere a Prelucrării Datelor cu Caracter Personal, www.dataprotection.ro.
</hr>
<br><br>
<a target="blank" href="https://didatec-my.sharepoint.com/:w:/g/personal/daraban_fl_bianca_utcluj_didatec_ro/ESZLn94USjtLojzvb-kNkT8BNofHBGAauTSjT6BRqav4HQ?e=wWhTlD">
	<button class="btn btn-warning">Analiza DPIA</button>
</a>
</body>
