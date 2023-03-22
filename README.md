# bootcampone
## Cvičení bootcamp1

### **GIT** 

1. Vytvořte si na GITHUBu novou repozitory / *done*
2. Naclonujte si ho k sobě pomocí Gitbash / *done* 
3. Nahrat do slozky nejake soubory / *done*
4. Vytvořte novou větev (Názvy větví volte vhodně, stejně tak commit message.), v ní proveďte nějaké změny a při mergování zpět nasimulujte merge conflict a ten vyřešte / *done*
5. Opakujte bod 4, ale místo mergování jen vytvořte pull request, poznamenejte si jeho link / *done*, link - https://github.com/mndvorakova/bootcampone/pull/1 pres GUI, druhy pull request - https://github.com/mndvorakova/bootcampone/compare/third?expand=1 
6. Smažte větev z bodu 4, lokálně ale i na serveru / *done* 
7. Zkuste si do nové větve dostat jeden nově vytvořený commit v masteru (který v té větvi ještě není), pomocí git cherry-pick / *done*
8. v rootu repozitory si vytvořte readme.md soubor a naplňte ho nějakým vlastním obsahem. Zkuste dle nápovědy všechny možnosti formátování. / *done*
9. Nechceme do repozitory pustit JPG a PNG obrázky - přidejte do gitignore / done
10. Nastavte si u nějakého commitu jeden TAG / done
11. (volitelně, není nutné) Zkuste .gitconfig nastavit tak, aby soubory s příponou .txt bral jako binární. Pak zkuste udělat v txt souboru změnu a podívejte se, jak jí GIT uvidí. (co pak takový merge změn v TXT souboru? :-) )


> Váš TL zjistí, kdo z kolegů bude úkol vyhodnocovat. Tomu pak umožněte přístup do repozitory pro kontrolu. Je to součástí vypracování úkolu


Git commands used in this exercise / examples:
```
git status
git add
git commit
git branch <name of the branch>
git cherry-pick
```

### **Jenkins**

    Použijte Tesena Jenkins, běží na URL: http://testlab.tesena.com:8080/ - jméno i heslo: bootcamp (technické problémy řešte s Tomášem Hákem)
    Vytvořte nový freestyle job se jménem "TechnicalSkills_VaseJmenoBezMezer"
    Job by měl:
    běžet každý všední den v 10h ráno (CRON)
    mít dva vstupní stringové parametry ENV a LANG 
    si stáhnout vaší GIT repozitory
    před každým buildem smazat workspace
    mít nastaveno, že po 5 buildech nebo 10 dnech se budou výsledky mazat.
    spustit shell (na pozadí testlabu je Linux stroj)
    vypsat adresář
    vytvořit nový soubor output.log s obsahem těch dvou vstupních proměnných a nějakého vašeho libovolného textu (echo ..... >> .... )
    ten libovolný soubor archivovat jako artefakt.


