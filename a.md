# A

1. Iniciar el desarrollo en ramas independientes: 

            git checkout main 
            git pull origin main 
            git checkout -b feature/featureA 

            git add . 
            git commit -m "Implementar historia de usuario 1" 
            git push origin feature/featureA 

2. Entregar desarrollos: 

            git  add . 
            git commit –m “entrega de desarrollos finales” 
            git push origin feature/featureA 

            git checkout main 
            git pull origin main 
            git merge feature/featureA 
            git push origin main 

3. Testear desarrollos: 

            git checkout main 
            git pull origin main 
            git checkout -b uat/testing 
            git merge feature/featureA 
            git merge feature/featureB 

4. Publicar una versión: 

            git checkout uat 
            git pull origin uat 
            git checkout -b release/v1.0  

            git add . 
            git commit -m "Prepare for release v1.0" 
            git tag -a v1.0 -m "Release version 1.0" 
            git push origin release/v1.0 
            git push origin v1.0 

            git checkout main
            git pull origin main
            git merge release/v1.0
            git push origin main
 
            git checkout uat
            git pull origin uat
            git merge release/v1.0
            git push origin uat

