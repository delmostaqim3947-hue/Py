# Structure : [ [nom, age, note], [nom, age, note], ... ]
classe = [
    ["Alice", 20, 15.5],
    ["Bob", 19, 12.0],
    ["Charlie", 22, 16.0]
]
def afficher_classe(classe):
    if not classe:
        print("La classe est vide.")
    else:
        for i, (nom, age, note) in enumerate(classe, start=1):
            print(f"{i}. {nom} - {age} ans - Note: {note}")
            # Exemple pour modifier le nom du premier étudiant
classe[0][0] = "Alice Nouvelle"
