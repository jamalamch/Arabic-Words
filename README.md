
# Arabic words

## All Arabic words from 3 to 9 letters

More than 12 million words divided by the number of letters and the type of letter for easy finding

> قائمة ب 1272533 كلمة عربية تم جمعها من أكثر من 650 كتابا قديما وحديثا  
> This project is a fork of 
>[ OSINTAI / Arabic_Words](https://github.com/OSINTAI/Arabic_Words)


جميع كلمات اللغة العربية من 3 احرف ل 9 احرف
تكتر من 8 مليون كلمة
الكلمات مقسمة على جداول على حسب الحرف و طول الكلمة


#### Java Code Exemple :

```sh

/** Determine if the word exists in the Arabic language.
* @param mot The word
* @return {@code true} if the word is present; {@code false} If the word does not exist. */
public static boolean ChercherLesMots(String mot) throws  SQLiteGdxException{
		String nBase = NomeTableDone(mot.charAt(0), mot.length());
	    if(dbHandler.rawQuery("SELECT MOT FROM `"+nBase+"` WHERE `mot` LIKE '"+mot+"' ").next())
	    	return true;
	    else
        return false;
}


/** Find the table for a word that begins with the letter char and the length.
* @param char The first letter of the word
* @param length The Word length
* @return The name of Table Who contains the word */
public static String NomeTableDone(char char, int length) {
		switch (char) {
		case 'ب':
			return "BAA" + L;
		case 'ت':
			return "TAA" + L;
		case 'ث':
			return "LAM" + L;
		case 'ج':
			return "GEM" + L;
		case 'ح':
			return "HAA" + L;
		case 'خ':
			return "KHA" + L;
		case 'د':
			return "DAL" + L;
		case 'ذ':
			return "ZAL" + L;
		case 'ر':
			return "RAA" + L;
		case 'ز':
			return "ZAY" + L;
		case 'س':
			return "SEN" + L;
		case 'ش':
			return "SHN" + L;
		case 'ص':
			return "SAD" + L;
		case 'ض':
			return "DAD" + L;
		case 'ط':
			return "TAA" + L;
		case 'ظ':
			return "DAD" + L;
		case 'ع':
			return "AIN" + L;
		case 'غ':
			return "GHN" + L;
		case 'ف':
			return "FAA" + L;
		case 'ق':
			return "QAF" + L;
		case 'ك':
			return "KAF" + L;
		case 'ل':
			return "LAM" + L;
		case 'م':
			return "MEM" + L;
		case 'ن':
			return "NON" + L;
		case 'ه':
			return "HAA" + L;
		case 'و':
			return "WAW" + L;
		case 'ي':
			return "YAA" + L;
		}
		return "ALF" + L;
}
```
