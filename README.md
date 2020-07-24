
## All Arabic words from 3 to 9 letters

More than 8 million words divided by the number of letters and the type of letter for easy finding



جميع كلمات اللغة العربية من 3 احرف ل 9 احرف
تكتر من 8 مليون كلمة
الكلمات مقسمة على جداول على حسب الحرف و طول الكلمة


#### Java Code Exemple :

```sh
public static boolean ChercherLesMots(String mots) throws  SQLiteGdxException{
		String nBase = NomeBaseDone(mots.charAt(0), mots.length());
	    if(dbHandler.rawQuery("SELECT MOT FROM `"+nBase+"` WHERE `mot` LIKE '"+mots+"' ").next())
	    	return true;
	    else
        return false;
}
public static String NomeBaseDone(char C, int L) {
		switch (C) {
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
