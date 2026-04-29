# planning pour le réseaux Afpa


Liste des tâches à réaliser:
- Schéma de l'infrastructure
- Création du plan d'adressage IP
- Mise en place du controleur de domaine
- Mise en place du firewall 
- Mise en place du DHCP
- Mise en place de l'active directory
- création des groupes + autorisations
- création des repertoire partagés 
- automatisation pour se connecter au répertoire partager
-
- ...
- Tests


```mermaid
        gantt
        dateFormat  YYYY-MM-DD
        title Planning de déploiement

        Schéma de l'infrastructure        :done,    t1, 2026-04-27,1d
        Création du plan d'adressage IP   :    t2, after t1, 1d
        Mise en place du controleur de domaine       :    t3, after t2, 5d
        Mise en place du firewall       :    t4, after t3, 5d
        Mise en place du DHCP     :    t5, after t4, 5d
        Mise en place de l'active directory    :    t6, after t5, 1d
        création des utilisateur et groupes + autorisations   :    t7, after t6, 1d
        automatisation pour se connecter au répertoire partager    :    t8, after t7, 1d



        
```




### Shéma de l'infrastructure


![commentaire](Image/réseau.png)



![commentaire](Image/droits.drawio.png )

###  Création du plan d'adressage IP
|               | adresse ip   | masque        | utilisateurs | superviseurs | agents | getway       | dns               | serveurs     | plage d’adresse     |
|---------------|--------------|---------------|--------------|--------------|--------|--------------|-------------------|--------------|---------------------|
| réseau        | 192.168.60.0 | 255.255.255.0 | 14           | 4            | 10     | 192.168.60.1 | Afpa-amiens.local | 192.168.60.1 | 192.168.60.50 à 100 |
| informatiique |              | 255.255.255.0 | 2            | 1            | 1      | 192.168.60.1 | Afpa-amiens.local | 192.168.60.1 | 192.168.60.50 à 100 |
| production    |              | 255.255.255.0 | 4            | 1            | 3      | 192.168.60.1 | Afpa-amiens.local | 192.168.60.1 | 192.168.60.50 à 100 |
| commercial    |              | 255.255.255.0 | 4            | 1            | 3      | 192.168.60.1 | Afpa-amiens.local | 192.168.60.1 | 192.168.60.50 à 100 |
| Comptabilité  |              | 255.255.255.0 | 4            | 1            | 3      | 192.168.60.1 | Afpa-amiens.local | 192.168.60.1 | 192.168.60.50 à 100 |