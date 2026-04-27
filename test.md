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