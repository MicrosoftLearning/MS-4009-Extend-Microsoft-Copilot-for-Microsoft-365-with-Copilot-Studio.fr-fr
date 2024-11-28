# Exercice : créer une action conversationnelle

Dans cet exercice, vous allez créer une action conversationnelle qui fournit des informations sur un projet organisationnel fictif intitulé « Project ABC ».

Tâches de l’exercice :

- Créer une action conversationnelle dans Copilot Studio
- Publier une action conversationnelle sur Microsoft Copilot
- Tester votre action conversationnelle dans Microsoft Copilot

## Tâche 1 : (facultatif) tester l’expérience par défaut

Pour commencer, posez une question sur le projet ABC dans Microsoft 365 Copilot.

1. Ouvrez **Microsoft Teams** et connectez-vous avec votre compte professionnel ou scolaire.

1. Sélectionnez **Conversation** dans la barre latérale.

1. Sélectionnez **Copilot** dans le menu de conversation.

1. Dans la zone de rédaction du message, entrez `Who should I contact for questions about Project ABC?`

1. Notez que Microsoft 365 Copilot n’a actuellement aucune information sur le project ABC.

## Tâche 2 : créer une action conversationnelle

Tout d’abord, configurez le nom, la solution et le schéma d’une nouvelle action conversationnelle dans Microsoft Copilot.

1. Dans votre navigateur web, accédez à [Copilot Studio](https://copilotstudio.microsoft.com) et connectez-vous avec votre compte professionnel ou scolaire, si vous y êtes invité.  Sélectionnez **Ignorer** pour ignorer les messages d’accueil.

    **Remarque :** la première fois que vous ouvrez Copilot Studio, il peut afficher une interface de conversation pour créer votre premier copilote. Si cela se produit, sélectionnez le menu **...** en haut à droite (en regard du bouton **Créer**), puis sélectionnez **Annuler la création du copilote**, puis **quittez** l’interface de conversation et affichez la page d’accueil de Copilot Studio.
1. Sélectionnez **Bibliothèque** dans le volet de navigation de gauche. Ici, vous pouvez afficher une liste d’actions et de connecteurs existants et en créer.
1. Sélectionnez **Ajouter un élément** en haut.  Un menu répertorie 2 options d’extension de Copilot pour Microsoft 365.
:::image type="content" source="../Media/extend copilot options.png" alt-text="La fenêtre répertorie 2 options d’extension de Copilot : créer un copilote ou créer une action.":::
1. Sélectionnez **Nouvelle action**.

1. Sélectionnez **Conversationnelle** pour créer une action conversationnelle.

1. Dans le champ **Nom**, entrez `Project ABC` et acceptez la solution et le schéma par défaut.

1. Sélectionnez **Créer** pour continuer. Votre nouvelle action conversationnelle est créée. L’attente peut durer plusieurs secondes. Lorsque vous avez terminé, vous êtes redirigé vers le canevas de création pour continuer à configurer votre action.

## Tâche 3 : configurer la rubrique

Ensuite, configurez le nom et le déclencheur de la rubrique.

1. Dans le volet création d’actions conversationnelles, accédez à l’onglet **Rubriques**.

1. Sélectionnez la zone de texte **Nom de la rubrique** en haut du volet, qui correspond par défaut au nom `"Untitled"` et entrez `Project ABC info` pour nommer la rubrique.

1. Dans le nœud **Déclencheur** de la rubrique, sélectionnez la zone de texte sous le texte « Décrivez ce que fait la rubrique », puis entrez `Answers questions and provides information about Project ABC, including questions about objectives, points of contact, and rollout timeline.`.

## Tâche 4 : envoyer un message

Ensuite, ajoutez un nœud à la rubrique pour envoyer un message sur le project ABC.

1. Sous le nœud Déclencheur, sélectionnez l’icône **+** pour ajouter un nouveau nœud.

1. Dans le menu affiché, sélectionnez **Envoyer un message**.  Un nœud de message est créé.

1. Dans le nœud de message, sélectionnez la zone de texte et entrez `Project ABC is an initiative aimed at improving the culture and engagement within the company.  Objectives of the project include improved morale, increased employee survey results, and improved culture ratings.  For more information about Project ABC, contact Devon Torres.`.

1. Sélectionnez **Enregistrer** au-dessus du canevas de création pour enregistrer les modifications.

## Tâche 5 : publier l’action

Ensuite, publiez l’action à utiliser dans Microsoft 365 Copilot.

1. Cliquez sur **Publier** en haut de la page.

1. Dans la page **Publier un plug-in**, sélectionnez **Publier**.

1. Dans la page **Publier le dernier contenu ?**, vérifiez que le plug-in d’informations sur le project ABC Info est activé et sélectionnez **Publier**.  La publication peut prendre quelques minutes.  Une notification s’affiche en haut de la fenêtre lorsque la publication est terminée.

## Tâche 6 : activer et tester l’action

Enfin, testez l’action dans Microsoft 365 Copilot.

1. Ouvrez **Microsoft Teams**.

1. Sélectionnez **Conversation** dans la barre latérale.

1. Sélectionnez **Copilot** dans le menu de conversation.

1. Dans la zone de rédaction du message, sélectionnez le bouton **Gérer la réponse de Copilot**.

1. Dans le menu volant, recherchez **Copilot Studio**, puis sélectionnez **Ajouter** pour ajouter Copilot Studio.
 
2. L’action **Informations de project ABC** doit maintenant être répertoriée dans le menu volant.  Vérifiez qu’**Informations de project ABC** est activé, puis fermez le menu volant.

:::image type="content" source="../Media/projectABCInfo-action-enabled.png" alt-text="Capture d’écran de l’action Informations de project ABC répertoriée dans le "Manage Copilot response" flyout in Teams.":::

3. Dans la zone de rédaction du message, entrez `Who should I contact for questions about Project ABC?`

4. Notez que Microsoft 365 Copilot renvoie les informations sur le project ABC en appelant l’action conversationnelle.

Vous pouvez personnaliser ou développer cette action conversationnelle avec des nœuds supplémentaires.  Par exemple, vous pouvez créer un nœud de **réponses génératives** et charger un fichier, en élargissant les connaissances disponibles pour l’action.

**Remarque :** n’oubliez pas ce qui suit lors du test de votre action dans Copilot :
- Copilot réécrit toujours vos réponses avec son propre style. Il n’est pas possible dans cette version préliminaire de transmettre le contenu tel quel à l’utilisateur final.
- La description de votre action conversationnelle est essentielle pour déterminer la fiabilité avec laquelle elle sera appelée. La description indique à l’orchestrateur les atouts de votre action et les réponses qu’elle peut fournir. Assurez-vous d’utiliser une prose claire lors de la rédaction de la description et envisagez d’expérimenter des modifications pour obtenir le meilleur résultat.
- Le suivi de ces étapes ne garantit pas que Copilot retourne les résultats attendus à chaque fois.  Copilot détermine quand appeler votre plug-in et comment retourner les résultats.

## (Facultatif) Défi : créer la votre

Appliquez ce que vous avez appris pour créer, publier et tester une nouvelle action conversationnelle pour un scénario de votre choix.  Passez en revue les étapes de cet exercice si nécessaire.