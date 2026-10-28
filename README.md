# ibalkosmou-art.github.io
موسى للمعلومات | Moussa for Informatics
# Démarrage rapide pour GitHub Codespaces

Démarrez rapidement avec GitHub Codespaces.

## Introduction

Dans ce guide, vous allez créer un codespace à partir d’un modèle de référentiel et explorer certaines des fonctionnalités essentielles disponibles dans le codespace. Vous allez travailler dans la version du navigateur de Visual Studio Code, qui est initialement l’éditeur par défaut pour GitHub Codespaces. Après avoir essayé ce guide de démarrage rapide, vous pouvez utiliser Codespaces dans d’autres éditeurs et modifier l’éditeur par défaut. Des liens sont fournis à la fin de ce guide.

À partir de ce guide de démarrage rapide, vous allez découvrir comment créer un codespace, vous connecter à un port transféré pour voir votre application s’exécuter, publier votre codespace dans un nouveau dépôt et personnaliser votre configuration avec des extensions.

Pour plus d’informations sur le fonctionnement GitHub Codespaces exact, consultez le guide complémentaire [Présentation approfondie de GitHub Codespaces](/fr/codespaces/about-codespaces/deep-dive).

## Création de votre codespace

1. Accédez au dépôt de modèles [github/haikus-for-codespaces](https://github.com/github/haikus-for-codespaces).
2. Cliquez sur **Utiliser ce modèle**, puis sur **Ouvrir dans un codespace**.

   ![Capture d’écran du bouton « Utiliser ce modèle » et du menu déroulant développé pour afficher l’option « Ouvrir dans un codespace ».](/assets/images/help/repository/use-this-template-button.png)

## Exécution de l'application

Une fois le codespace créé, le dépôt de modèles est automatiquement cloné dans celui-ci. Vous pouvez maintenant exécuter l’application et la lancer dans un navigateur.

1. Lorsque le terminal devient disponible, entrez la commande `npm run dev`. Cet exemple utilise un projet Node.js et cette commande exécute le script intitulé « dev » dans le fichier `package.json`, qui démarre l’application web définie dans l’exemple de dépôt.

   ![Capture d’écran du terminal dans VS Code avec la commande « npm run dev » entrée.](/assets/images/help/codespaces/codespaces-npm-run-dev.png)

   S’il s’agit d’un autre type d’application, entrez la commande de démarrage correspondante pour ce projet.

2. Quand votre application démarre, le codespace reconnaît le port sur lequel l’application s’exécute et affiche un message contextuel pour vous informer que le port a été transféré.

   ![Capture d’écran du message contextuel : « Votre application exécutée sur le port 3000 est disponible ». En dessous se trouve un bouton vert intitulé « Ouvrir dans le navigateur ».](/assets/images/help/codespaces/quickstart-port-toast.png)

3. Cliquez sur **Ouvrir dans le navigateur** pour afficher votre application en cours d’exécution dans un nouvel onglet.

## Modifier l’application et afficher les modifications

1. Revenez à votre codespace et ouvrez le fichier `haikus.json` en cliquant dessus dans l’Explorateur.

2. Modifiez le champ `text` du premier haiku pour personnaliser l’application avec votre propre haiku.

3. Revenez à l’onglet de l’application en cours d’exécution dans votre navigateur et actualisez pour afficher vos modifications.

<svg version="1.1" width="16" height="16" viewBox="0 0 16 16" class="octicon octicon-light-bulb" aria-label="light-bulb" role="img"><path d="M8 1.5c-2.363 0-4 1.69-4 3.75 0 .984.424 1.625.984 2.304l.214.253c.223.264.47.556.673.848.284.411.537.896.621 1.49a.75.75 0 0 1-1.484.211c-.04-.282-.163-.547-.37-.847a8.456 8.456 0 0 0-.542-.68c-.084-.1-.173-.205-.268-.32C3.201 7.75 2.5 6.766 2.5 5.25 2.5 2.31 4.863 0 8 0s5.5 2.31 5.5 5.25c0 1.516-.701 2.5-1.328 3.259-.095.115-.184.22-.268.319-.207.245-.383.453-.541.681-.208.3-.33.565-.37.847a.751.751 0 0 1-1.485-.212c.084-.593.337-1.078.621-1.489.203-.292.45-.584.673-.848.075-.088.147-.173.213-.253.561-.679.985-1.32.985-2.304 0-2.06-1.637-3.75-4-3.75ZM5.75 12h4.5a.75.75 0 0 1 0 1.5h-4.5a.75.75 0 0 1 0-1.5ZM6 15.25a.75.75 0 0 1 .75-.75h2.5a.75.75 0 0 1 0 1.5h-2.5a.75.75 0 0 1-.75-.75Z"></path></svg> Si vous avez fermé l’onglet du navigateur, cliquez sur l’onglet VS CodePorts, pointez sur la valeur **d’adresse locale** du port en cours d’exécution, puis cliquez sur l’icône **Ouvrir dans le navigateur** .

![Capture d’écran du volet « Ports ». L’onglet « Ports » et une icône de globe, qui ouvre le port transféré dans un navigateur, sont mis en évidence avec des encadrés en orange.](/assets/images/help/codespaces/quickstart-forward-port.png)

## Validation (commit) et envoi (push) de vos modifications

Maintenant que vous avez apporté quelques modifications, vous pouvez utiliser le terminal intégré ou la vue source pour publier votre travail dans un nouveau dépôt.

1. Dans la barre d’activités, cliquez sur la vue **Contrôle de code source**.

   ![Capture d’écran de la barre d’activités VS Code avec le bouton Contrôle de code source mis en surbrillance avec un encadré orange.](/assets/images/help/codespaces/source-control-activity-bar-button.png)

2. Pour indexer vos modifications, cliquez sur <svg version="1.1" width="16" height="16" viewBox="0 0 16 16" class="octicon octicon-plus" aria-label="Stage Changes" role="img"><path d="M7.75 2a.75.75 0 0 1 .75.75V7h4.25a.75.75 0 0 1 0 1.5H8.5v4.25a.75.75 0 0 1-1.5 0V8.5H2.75a.75.75 0 0 1 0-1.5H7V2.75A.75.75 0 0 1 7.75 2Z"></path></svg> à côté du fichier `haikus.json`, ou à côté de **Modifications** si vous avez modifié plusieurs fichiers et que vous souhaitez tous les indexer.

   ![Capture d’écran de la barre latérale « Contrôle de code source » avec le bouton de mise en scène (signe plus), à droite de « Modifications », mis en évidence avec un contour orange foncé.](/assets/images/help/codespaces/codespaces-commit-stage.png)

3. Pour valider vos modifications mises en scène, tapez un message de validation décrivant la modification que vous avez apportée, puis cliquez sur **Valider**.

   ![Capture d’écran de la barre latérale « Contrôle de code source ». Le message de commit, « Modifier le texte et les styles du haïku », et le bouton « Commit » sont mis en évidence en orange.](/assets/images/help/codespaces/vscode-commit-button.png)

4. Cliquez sur **Publier la branche**.

   ![Capture d’écran de la barre latérale « Gestion de code source » montrant le bouton « Publier la branche ».](/assets/images/help/codespaces/vscode-publish-branch-button.png)

5. Dans la liste déroulante « Nom du référentiel », tapez un nom pour votre nouveau référentiel, puis sélectionnez **Publier dans GitHub un référentiel privé** ou **Publier dans GitHub un référentiel public**.

   ![Capture d’écran du menu déroulant du nom du référentiel dans VS Code. Deux options s’affichent pour publier sur un dépôt privé ou public.](/assets/images/help/codespaces/choose-new-repository.png)

   Le propriétaire du nouveau référentiel sera le GitHub compte avec lequel vous avez créé l’espace de code.

6. Dans la fenêtre contextuelle qui s’affiche dans le coin inférieur droit de l’éditeur, cliquez **sur GitHubOuvrir** pour afficher le nouveau référentiel sur GitHub. Dans le nouveau dépôt, affichez le fichier `haikus.json` et vérifiez que la modification que vous avez apportée dans votre codespace a bien été poussée dans le dépôt.

   ![Capture d’écran d’un message de confirmation d’un dépôt publié avec succès, montrant le bouton « Ouvrir dans GitHub ».](/assets/images/help/codespaces/open-on-github.png)

## Personnalisation avec une extension

Lorsque vous vous connectez à un espace de code à l’aide du navigateur ou de l’application Visual Studio Code de bureau, vous pouvez accéder à la Visual Studio Code Place de marché directement à partir de l’éditeur. Pour cet exemple, vous allez installer une VS Code extension qui modifie le thème, mais vous pouvez installer n’importe quelle extension utile pour votre flux de travail.

1. Dans la barre d’activités, cliquez sur l’icône Extensions.

   ![Capture d’écran de la barre d’activités. L’icône Extensions est mise en évidence avec un encadré orange.](/assets/images/help/codespaces/extensions-activity-bar-icon.png)

2. Dans la barre de recherche, tapez `fairyfloss` et cliquez sur **Installer**.

   ![Capture d’écran de « Extensions : Place de marché ». La zone de recherche affiche « fairyfloss ». Les résultats affichent l’extension « fairyfloss » avec un bouton « Installer ».](/assets/images/help/codespaces/add-extension.png)

3. Sélectionnez le thème `fairyfloss` en le sélectionnant dans la liste.

   ![Capture d’écran de la liste déroulante « Sélectionner le thème de couleur », avec le thème « fairyfloss » sélectionné.](/assets/images/help/codespaces/fairyfloss.png)

### À propos de la synchronisation des paramètres

Vous pouvez activer la synchronisation des paramètres pour synchroniser les extensions et d’autres paramètres entre les appareils et les instances de VS Code.
Vos paramètres synchronisés sont mis en cache dans le cloud. Si la synchronisation des paramètres est activée dans un codespace, toutes les mises à jour que vous apportez à vos paramètres dans le codespace sont envoyées vers le cloud et toutes les mises à jour que vous envoyez au cloud à partir d’un autre emplacement sont extraites de votre codespace. Pour plus d’informations, consultez [Personnaliser GitHub Codespaces pour votre compte](/fr/codespaces/setting-your-user-preferences/personalizing-github-codespaces-for-your-account#settings-sync).

## Étapes suivantes

Vous avez créé, personnalisé et exécuté avec succès votre première application dans un codespace. Il vous reste encore beaucoup de choses à découvrir. Voici quelques ressources utiles pour effectuer vos prochaines étapes avec GitHub Codespaces.

* [Présentation approfondie de GitHub Codespaces](/fr/codespaces/about-codespaces/deep-dive) : Ce guide de démarrage rapide présente certaines des fonctionnalités de GitHub Codespaces. La présentation approfondie examine ces domaines d’un point de vue technique.
* [Ajout d’une configuration de conteneur de développement à votre dépôt](/fr/codespaces/setting-up-your-project-for-codespaces/adding-a-dev-container-configuration) : Ces guides fournissent des informations sur la configuration de votre référentiel à utiliser GitHub Codespaces avec des langues spécifiques.
* [Présentation des conteneurs de développement](/fr/codespaces/setting-up-your-project-for-codespaces/adding-a-dev-container-configuration/introduction-to-dev-containers) : Ce guide fournit des détails sur la création d’une configuration personnalisée pour Codespaces votre projet.

## Pour aller plus loin

* [Activation ou désactivation de GitHub Espaces de code pour votre organisation](/fr/codespaces/managing-codespaces-for-your-organization/enabling-or-disabling-github-codespaces-for-your-organization)
* [Utilisation des espaces de code GitHub dans Visual Studio Code](/fr/codespaces/developing-in-a-codespace/using-github-codespaces-in-visual-studio-code)
* [Utilisation de GitHub Codespaces avec GitHub CLI](/fr/codespaces/developing-in-a-codespace/using-github-codespaces-with-github-cli)
* [Définition de votre éditeur par défaut pour GitHub Espaces de code](/fr/codespaces/setting-your-user-preferences/setting-your-default-editor-for-github-codespaces)
* [Gestion du coût de GitHub Espaces de code dans votre organisation](/fr/codespaces/managing-codespaces-for-your-organization/managing-the-cost-of-github-codespaces-in-your-organization)
