# Exercice : créer une action de connecteur

Dans cet exercice, vous allez :

- Créer une action de connecteur dans Copilot Studio
- Tester l’action du connecteur dans Microsoft Teams
- Enregistrer et publier l’action du connecteur

## Tâche 1 : créer une action de connecteur dans Copilot Studio

Dans cette tâche, vous allez configurer une action de connecteur pour le connecteur MSN Météo.

1. Accédez à [Copilot Studio](https://copilotstudio.microsoft.com) et connectez-vous avec votre compte professionnel ou scolaire, si vous y êtes invité. Ignorez les messages de bienvenue.

    **Remarque :** la première fois que vous ouvrez Copilot Studio, il peut afficher une interface de conversation pour créer votre premier copilote. Si cela se produit, sélectionnez le menu **...** en haut à droite (en regard du bouton **Créer**), puis sélectionnez **Annuler la création du copilote** pour quitter l’interface de conversation et afficher la page d’accueil de Copilot Studio.
1. Sélectionnez **Bibliothèque** dans le volet de navigation de gauche. Ici, vous pouvez afficher une liste d’actions et de connecteurs existants et en créer.
1. Sélectionnez **Ajouter un élément** en haut.  Un menu répertorie 2 options d’extension de Copilot pour Microsoft 365.
:::image type="content" source="../Media/extend copilot options.png" alt-text="La fenêtre répertorie 2 options d’extension de Copilot : créer un copilote ou créer une action.":::
2. Sélectionnez **Nouvelle action**.
3. Sélectionnez **Connecteur** pour ouvrir l’Assistant pour les actions du connecteur.
4. Sélectionnez **MSN Météo** comme connecteur.
5. **Passez en revue** la description.

    > [!IMPORTANT]
    > Cette description est très importante, car Copilot l’utilisera pour faire correspondre le message de l’utilisateur à votre plug-in. Si vous ne disposez pas d’une bonne description, Copilot risque de ne pas déclencher votre action de connecteur.

1. Cliquez sur **Suivant**.
1. Sélectionnez l’action **Obtenir la météo actuelle**.
1. **Passez en revue** la description de l’action.

    > [!IMPORTANT]
    > Passez en revue la description de l’action dans l’écran suivant. Cette description de l’action est très importante, car Copilot l’utilisera pour faire correspondre le message de l’utilisateur à votre action. Si vous ne disposez pas d’une bonne description de l’action, Copilot risque de déclencher la mauvaise action.

1. Cliquez sur **Suivant**.
1. **Passez en revue** les descriptions de toutes les entrées et sorties.

    > [!IMPORTANT]
    > Passez en revue les descriptions des entrées et des sorties dans l’écran suivant. Ces descriptions des entrées et des sorties sont très importantes, car Copilot les utilisera pour déclencher le connecteur (entrées) et pour vous écrire une bonne réponse (sorties). Si vous ne disposez pas de bonnes descriptions des entrées et des sorties, Copilot risque de ne pas déclencher correctement le connecteur ou il ne renvoie pas une bonne réponse.

1. Cliquez sur **Suivant**.
1. Ensuite, vous verrez un écran dans lequel vous pouvez ajouter d’autres actions si vous le souhaitez, mais dans ce cas, nous allons ignorer cette étape et sélectionner **Suivant**.

## Tâche 2 : tester l’action du connecteur dans Microsoft Teams

Dans cette tâche, vous allez tester l’action du connecteur que vous avez configurée à la tâche 1 dans Microsoft 365 Copilot dans Microsoft Teams.

![La section de révision, test et publication de votre action dans l’Assistant Action du connecteur.](../Media/connect-test.png)

1. Sélectionnez une connexion existante si vous en avez une, ou sélectionnez **Nouvelle connexion** pour créer une connexion pour le connecteur MSN Météo
1. Dans le menu **Nouvelle connexion**, sélectionnez **Créer**.
1. Sous **Connexion sélectionnée**, vous pouvez maintenant sélectionner votre nouvelle connexion dans le menu déroulant.
1. Sélectionnez le bouton **Tester l’action**.

    > [!NOTE]
    > Cela déclenche un processus dans lequel votre action de connecteur est déployée sur Microsoft Teams afin de pouvoir la tester.

1. Sélectionnez **Ouvrir pour test** pour effectuer le test.

    > [!NOTE]
    > Cela ouvre un nouvel onglet de navigateur et tente de lancer Microsoft Teams.

1. N’hésitez pas à sélectionner **Annuler** dans la fenêtre contextuelle où il tente de lancer Microsoft Teams.
1. Sélectionnez **Utiliser l’application web à la place**.

    > [!NOTE]
    > Cela ouvre Microsoft 365 Copilot dans Microsoft Teams.

1. Dans la zone de rédaction du message de Copilot dans Teams, sélectionnez l’icône du **plug-in** en regard de l’icône d’envoi.
1. Recherchez le plug-in **Test-MSN Météo** et sélectionnez le bouton bascule pour l’activer.

    > [!NOTE]
    > Le message suivant s’affiche.

    ![Le message indique que le plug-in Test-MSN Météo est activé.](../Media/test-msn-weather.png)


1.  Envoyez le message suivant à Microsoft 365 Copilot, en remplissant les valeurs de votre emplacement et des unités souhaités.

    ```text
    What is the current weather in <your location> in <celsius/fahrenheit> according to MSN Weather?
    ```

1. Si tout s’est bien passé, Copilot doit répondre avec un message à l’aide du plug-in.  

   ![Capture d’écran d’un exemple de message et de réponse. Le plug-in renvoie le temps qu’il fait en ce moment à Utrecht, aux Pays-Bas, en degrés Celsius.](../Media/msn-weather-result.png)

   **Remarque :** Copilot peut vous demander l’autorisation avant d’utiliser le plug-in.  Sélectionnez **Toujours autoriser** pour autoriser Copilot à utiliser le plug-in.

   :::image type="content" source="../Media/test-msn-weather-allow.png" alt-text="Capture d’écran de Copilot demandant l’autorisation d’utiliser le plug-in.":::

## Tâche 3 : enregistrer et publier l’action du connecteur

Dans cette tâche, vous allez enregistrer l’action du connecteur et la publier.

Reprenons là où nous nous étions arrêtés dans Copilot Studio.

1. Sélectionnez **Suivant** dans l’Assistant et l’action du connecteur sera publiée.

    > [!NOTE]
    > Dans l’écran suivant, vous serez en mesure d’accéder à l’écran de détails ou d’enregistrer et fermer. Comme indiqué dans le message, l’action peut prendre quelques minutes à s’afficher dans les expériences de copilote.

      ![Capture d’écran de l’écran de publication dans l’Assistant Action du connecteur.](../Media/connector-action-finished.png)
   
1. Sélectionnez **Enregistrer et fermer**.

Vous avez maintenant configuré et publié votre action de connecteur.
