LAB 1 - Configuration Mobexler & Android

Étape 1 : Configuration Réseau VirtualBox

   Configuration de l'adaptateur 1 en mode NAT pour permettre l'accès à Internet depuis la VM.

 ![WhatsApp Image 2026-02-15 at 21 24 58](https://github.com/user-attachments/assets/e4f9f3f3-a762-4d35-a6da-e6ec4d33257d)
    
  Configuration de l'adaptateur 2 en mode Host-Only pour permettre la communication entre l'hôte et la VM.
  
 ![WhatsApp Image 2026-02-15 at 21 25 16](https://github.com/user-attachments/assets/7b83be50-9988-41d8-83b9-8dd949e0b27a)

 Étape 2 : Vérification Réseau dans Mobexler
 
   Vérification des interfaces réseau

 ![WhatsApp Image 2026-02-15 at 21 30 16](https://github.com/user-attachments/assets/0cf97103-531e-4135-9f84-390f2f21e98f)
 ![WhatsApp Image 2026-02-15 at 21 31 33](https://github.com/user-attachments/assets/5258da53-3848-4579-a527-3e908b7a1c19)
      
Étape 3 : Vérification de la connectivité Internet

 pour vérifier que la machine virtuelle a accès à Internet, nous avons utilisé les commandes suivantes :
 
  Test 1 : Ping vers une adresse IP publique (ping -c 2 8.8.8.8)

  Test 2 : Ping vers un nom de domaine (ping -c 2 google.com)

 ![WhatsApp Image 2026-02-15 at 21 33 15](https://github.com/user-attachments/assets/ff7d44c9-ef35-4021-86c0-749a401a3048)

 Étape 4 : Créer le snapshot “CLEAN” (baseline)
 
   Après avoir configuré correctement la machine virtuelle (import, configuration réseau NAT + Host-Only, vérification Internet et ADB), nous avons créé un snapshot afin de sauvegarder l’état stable de la VM.
   
   Nom de snapshot :
   
   CLEAN_BASELINE_TP1
   
   Description :
   
   Import OK, NAT + HostOnly OK, boot OK, prêt ADB
   
   Objectif :
   
   Permettre de restaurer rapidement la machine virtuelle en cas d’erreur ou de mauvaise manipulation.
   
 ![WhatsApp Image 2026-02-15 at 21 40 59](https://github.com/user-attachments/assets/0e807413-319a-431c-a811-5009593a3f34)

 Étape 5 — Connexion du téléphone Android à la VM (USB)
 
 Après activation du mode développeur et du débogage USB sur le téléphone, nous avons connecté l’appareil à la machine virtuelle.

 ![WhatsApp Image 2026-02-15 at 22 05 13](https://github.com/user-attachments/assets/7d9e2cef-a560-4c5e-b34f-3287d54a24f4)
 ![WhatsApp Image 2026-02-15 at 22 26 24](https://github.com/user-attachments/assets/2255bf83-69c9-4024-995a-0cc98cb15d70)
 ![WhatsApp Image 2026-02-15 at 22 12 51](https://github.com/user-attachments/assets/83aa4efc-9dc9-4af1-a964-7cdd75eb2327)

   La commande adb devices confirme que le téléphone Android est correctement connecté à la machine virtuelle, avec le statut "device", indiquant une connexion ADB fonctionnelle.

      


    

   
      
       




     


