+++
author = "DS"
date = 0001-01-01T00:00:00Z
description = ""
draft = true
slug = "cisco"
title = "Cisco"

+++


<script> 
function dec_bin(num){
	n = document.getElementById("decimale").value; 
	binario = "";

	while(n!=0) {
		resto = n%2; 
		n = (n-resto)/2; 
		binario = resto + binario;
	}
	
	return binario;
}


function dec_ott(num){
	n = document.getElementById("decimale").value; 
	ottale = "";

	while(n!=0) {
		resto = n%8; 
		n = (n-resto)/8;
		ottale = resto + ottale;
	}
	
	return ottale;
}

function dec_esa(num){
	n = document.getElementById("decimale").value; 
	esa = ""; 
	while(n!=0) { 
		resto = n%16; 
		n = (n-resto)/16; 
		ar = new Array('0','1','2','3','4','5','6','7','8','9','A','B','C','D','E','F');
		if (resto > 9) 
			resto = ar[resto]; 
		esa = resto + esa;
	}
	
	return esa;
}


function change(name)
{
		n = document.getElementById("decimale").value;
                result = dec_bin(n);
		result2 = dec_ott(n);
		result3 = dec_esa(n);
		risultato.value=result;
		risultato2.value=result2;
		risultato3.value=result3;
}
</script>

**Conversioni tra numeri con basi diverse**
 da decimale a binario

__
da binario a decimale
![images-1](http://35.228.152.175/content/images/2020/03/images-1.png)

_______________________________________________________________________________
da esadecimale a decimale
![esadecimale-bin-1](http://35.228.152.175/content/images/2020/03/esadecimale-bin-1.jpg)
__
da binario ad esadecimale

__
da esadecimale a binario



