# AWS CICD PIPELINE

- A projektnek csak a CI része van ledokumentálva
!
![](https://github.com/Harii75/AWS_CICD/blob/main/AWS/K%C3%A9perny%C5%91k%C3%A9p%202023-10-12%20175448.png?raw=true)
## Projekt célja:
Ebben a projektben egy egyszerű Flask alkalmazást implementálunk egy CI/CD pipeline-ba. Az alkalmazás kódját a CodeCommit használatával kezeljük, a CodeBuild segítségével építjük, a CodePipeline segítségével automatizáljuk a CI/CD folyamatot,CodeDeploy használatával telepítjük az alkalmazást egy EC2 VM-re.

## Lépések:
### 1. CodeCommit beállítása.

  Előszőr létrehozzuk a projektet. <br>
  <img src="https://github.com/Harii75/AWS_CICD/blob/main/AWS/codebuild-1.png" width=50% height=50%> 
  
  Ezt követően összekötjük a GitHub fiókunkat az CodeCommittal és kiválasztjuk a repot ahol a Flask appunk van.<br>
  <img src="./AWS/codebuild2.png" width=50% height=50%><br>

  Ezen a projeken Ubuntu fut <br>
  <img src="./AWS/codebuild3.png" width=50% height=50%><br>

  Majd a CodeCommithoz rendelt role-hoz hozzáadjuk a  "SSMFullAccess"-t policyt, hogy önállóan működni.
