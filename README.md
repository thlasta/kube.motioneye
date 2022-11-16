# kube.motioneye

echo "# kube.grafana" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:thlasta/kube.motioneye.git
git push -u origin main


# Repo clonen
git clone git@github.com:thlasta/kube.motioneye.git

# Repo auschecken/holen
git pull git@github.com:thlasta/kube.motioneye.git

# Bei Änderungen:
git commit -m "Änderungsbeschreibung"
git push --all

# Jump one folder up, and apply to the whole folder:
kubectl apply -f motioneye/

# Namespace "monitoring" anlegen
kubectl create namespace motioneye