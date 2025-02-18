# To-do-liste
En suivant cette feuille de route, vous pourrez vous assurer de ne rien oublier et de prendre chaque décision au moment opportun. 
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>To-Do Liste Ultra Complète pour un Mariage Réussi 📌</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: left; color: #02084b; background-color: white; padding: 20px; }
        h2 { color: #02084b; padding: 10px 0; font-size: 20px; margin: 0; }
        ul { list-style: none; padding: 0; }
        li { display: flex; align-items: center; margin: 5px 0; }
        input[type="checkbox"] { margin-right: 5px; }
    </style>
</head>
<body>
    <h1>To-Do Liste Ultra Complète pour un Mariage Réussi 📌</h1>
    
    <div id="todo-list"></div>
    
    <script>
        const tasks = {
            "12-9 Mois Avant le Mariage": [
                "Fixer la date et le lieu de la cérémonie et de la réception",
                "Définir le budget global",
                "Établir une liste préliminaire des invités",
                "Choisir un thème et une palette de couleurs",
                "Engager un wedding planner (si souhaité)",
                "Réserver les prestataires clés (traiteur, photographe, vidéaste, DJ, etc.)",
                "Commencer les recherches pour la robe de mariée et le costume",
                "Déposer le dossier administratif pour le mariage civil",
                "Bloquer les hébergements pour les invités venant de loin",
                "Établir un premier rétroplanning des préparatifs"
            ],
            "9-6 Mois Avant le Mariage": [
                "Finaliser la liste des invités",
                "Envoyer les \"Save the Date\"",
                "Choisir et commander la robe de mariée et les accessoires",
                "Réserver les prestataires secondaires (coiffeur, maquilleur, fleuriste…)",
                "Définir le menu avec le traiteur et prévoir une dégustation",
                "Réserver le véhicule des mariés et organiser le transport des invités",
                "Choisir le type de cérémonie et préparer les documents nécessaires",
                "Prévoir des animations et des surprises pour la soirée",
                "Élaborer le planning détaillé de la journée du mariage",
                "Commencer à réfléchir à la décoration et aux compositions florales"
            ],
            "6-4 Mois Avant le Mariage": [
                "Concevoir et commander les invitations officielles",
                "Choisir et réserver les tenues du cortège et des témoins",
                "Faire les premiers essais coiffure et maquillage",
                "Sélectionner les musiques de la cérémonie et de la réception",
                "Élaborer le plan de table provisoire",
                "Acheter ou louer les éléments de décoration",
                "Planifier l’enterrement de vie de jeune fille/garçon",
                "Vérifier les délais pour les documents légaux",
                "Réserver la lune de miel et organiser les formalités de voyage"
            ],
            "4-2 Mois Avant le Mariage": [
                "Envoyer les invitations et collecter les réponses",
                "Faire un essayage final de la robe et du costume",
                "Préparer les alliances",
                "Organiser une rencontre avec tous les prestataires pour finaliser les détails",
                "Acheter les accessoires de dernière minute (bijoux, chaussures…)",
                "Préparer la papeterie pour le mariage (menus, plans de table, livre d’or…)",
                "Confirmer la réservation du matériel loué (chaises, tentes, éclairages…)",
                "Préparer un kit d’urgence pour le jour J (épingle, pansements, maquillage…)",
                "Organiser la répétition de la cérémonie (si nécessaire)"
            ],
            "1 Mois Avant le Mariage": [
                "Réaliser les derniers essayages et ajustements de tenues",
                "Confirmer tous les prestataires et revoir le planning du jour J",
                "Finaliser le plan de table",
                "Établir la playlist avec le DJ et lui donner la liste des musiques interdites",
                "Vérifier les détails logistiques avec le lieu de réception",
                "Acheter et préparer les cadeaux pour les invités",
                "Confirmer le programme du jour J avec les témoins et la famille",
                "Vérifier que tous les paiements aux prestataires sont réglés"
            ],
            "1 Semaine Avant le Mariage": [
                "Vérifier que tout est prêt (tenues, alliances, papiers…)",
                "Faire un dernier point avec les prestataires",
                "Déléguer les dernières tâches à des proches",
                "Se détendre et prendre du temps pour soi",
                "Faire une pause et bien dormir avant le grand jour !"
            ],
            "Jour J 🎉": [
                "Se préparer et se détendre",
                "Profiter du moment avec ses proches",
                "Ne pas stresser pour les imprévus, tout est prévu !",
                "Dire OUI et savourer chaque instant ❤️"
            ]
        };

        function renderTasks() {
            const container = document.getElementById("todo-list");
            container.innerHTML = "";
            
            for (const category in tasks) {
                const section = document.createElement("div");
                section.innerHTML = `<h2>${category}</h2>`;
                
                const ul = document.createElement("ul");
                tasks[category].forEach(task => {
                    const li = document.createElement("li");
                    const checkbox = document.createElement("input");
                    checkbox.type = "checkbox";
                    
                    li.appendChild(checkbox);
                    li.appendChild(document.createTextNode(task));
                    ul.appendChild(li);
                });
                
                section.appendChild(ul);
                container.appendChild(section);
            }
        }

        renderTasks();
    </script>
</body>
</html>
