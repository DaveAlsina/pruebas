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
