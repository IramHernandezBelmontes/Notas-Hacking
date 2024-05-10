## Descripción
[keygenme-trial.py](https://mercury.picoctf.net/static/fb75b48f9214cf992a2199b5785564e7/keygenme-trial.py)
## Pistas 
none
## Solución

introducimos este codigo antes del metodo stardb trial y nos da la flag
def key_gen():

dynamic_part = []

nums = [4,5,3,6,2,7,1,8]

for x in nums:

dynamic_part.append(hashlib.sha256(bUsername_trial).hexdigest()[x])

print(key_full_template_trial.replace(key_part_dynamic1_trial, "".join(dynamic_part)))

exit(key_gen())
## Bandera
picoCTF{1n_7h3_|<3y_of_0d208392}