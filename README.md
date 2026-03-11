# securite-mobile-lab5x
## Outils nécessaires sont unzip et JADX

### les etaps
 ## instalation de GHIDRA :
<img width="1486" height="1036" alt="image" src="https://github.com/user-attachments/assets/e7256391-b0de-44df-827e-53cec554b1c3" />
## Unzip les fichiers 
<img width="1250" height="1006" alt="image" src="https://github.com/user-attachments/assets/86ac81c8-c363-43bc-90cd-265f25d74325" />

<img width="925" height="222" alt="image" src="https://github.com/user-attachments/assets/c45e34a7-b620-4ad0-acab-ac049005e3a1" />


<img width="726" height="1080" alt="image" src="https://github.com/user-attachments/assets/70bd9dd7-9c42-4d40-8730-7af7410d8c19" />  

  ## Étape 1 — Installer et lancer l’APK:Drop and drag lapp dans lemulateure 
<img width="662" height="901" alt="image" src="https://github.com/user-attachments/assets/142f0bf1-5c3d-43f5-9f93-a73b4e978994" />  

 ## Ou avec la commande   
 
   adb install UnCrackable-Level2.apk  
   

   <img width="676" height="110" alt="image" src="https://github.com/user-attachments/assets/acfef8be-a026-4f58-b72e-2a8f8eb959c9" />

# Linstalation reussit :
<img width="580" height="114" alt="image" src="https://github.com/user-attachments/assets/dbf9d71f-5d57-47b8-ba00-228d142dabac" />    

## lapp ne fonctione pas malgre tout les tentative et changementdes versions onnpasse a la prohaine etap   

  <img width="282" height="593" alt="image" src="https://github.com/user-attachments/assets/dd27c1a9-7d95-4cf4-8a3a-2b49ac75f61d" />  
  

## Étape 3 — Décompiler l’APK avec JADX  

# linstallation de JADX:  


<img width="1264" height="973" alt="image" src="https://github.com/user-attachments/assets/6c72d1c3-30a3-4a97-8c49-fe1ae55ab6a9" />     

# Lencement de JADX 

<img width="1133" height="552" alt="image" src="https://github.com/user-attachments/assets/56997921-ce99-4b0d-b36e-0cf0020080fe" />

## Activity main     
 
<img width="1160" height="1046" alt="image" src="https://github.com/user-attachments/assets/499e3878-5d66-4536-865b-1c5370f310fe" />  

  # Code Check 


    
<img width="384" height="166" alt="image" src="https://github.com/user-attachments/assets/90a02f9e-ae89-4a41-987c-2da30fb29c10" />  

  Le mot-clé native = le code est dans libfoo.so, pas en Java !  
  # Étape 7 — Importer libfoo.so dans Ghidra
<img width="516" height="437" alt="image" src="https://github.com/user-attachments/assets/af292b57-789c-4a68-bbbe-fec42e6b0d17" />

# lanaluse de fichier 
<img width="1688" height="792" alt="image" src="https://github.com/user-attachments/assets/16e746d8-b108-4307-aefa-387d2f837199" />  

# Apres lanalyse nous avons le code :  

<img width="802" height="792" alt="image" src="https://github.com/user-attachments/assets/86d74448-8177-4398-ae76-69dbe6519b69" />  

# Finalement Rsultat ettendue :    

<img width="364" height="52" alt="image" src="https://github.com/user-attachments/assets/e88001b0-e5ef-46bf-9c9a-6c77fbfe6a26" />

  Ce que Ghidra nous montre :  
  
1. La fonction `Java_sg_vantagepoint_uncrackable2_CodeCheck_bar` reçoit la chaîne de l'utilisateur
2. Elle copie le secret **"Thanks for all the fish"** dans un buffer local (`local_34`)
3. Elle compare avec `strncmp` la chaîne entrée avec le secret
4. Si elles sont identiques → retourne `true` → **"This is the correct secret."**
## ✅ Maintenant va tester dans l'app !

Sur l'émulateur, lance l'app et tape :
```
Thanks for all the fish
```
Mais lapp ne fonctionne pas 














