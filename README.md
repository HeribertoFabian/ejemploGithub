### Generar una nueva clave SSH
ssh-keygen -t ed25519 -C "tuemail@example.com"



### Agregar la clave SSH al agente SSH
eval "$(ssh-agent -s)"


### Agregar tu clave privada al agente SSH:
ssh-add ~/.ssh/id_ed25519


clip < ~/.ssh/id_ed25519.pub



git config --global user.name "Tu Nombre"
git config --global user.email "tuemail@example.com"



ssh -T git@github.com
