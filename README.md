# M365JejeAvalonia

# M365_Jéjé_Avalonia

## Description
M365_Jéjé_Avalonia est une application de gestion de tenants Microsoft 365 multi-plateforme (Windows et macOS), développée en C# avec le framework Avalonia 11.2.3. Elle permet d'exécuter des commandes PowerShell pour administrer des services Microsoft 365, comme Microsoft Graph, Exchange Online et Microsoft Teams.

## Fonctionnalités
- Connexion et déconnexion aux services Microsoft 365.
- Gestion des comptes utilisateurs.
- Gestion des groupes de sécurité.
- Gestion des équipes Teams.
- Configuration des calendriers de groupes.
- Gestion des conversations et des politiques de messagerie.
- Exécution de commandes PowerShell via un service PowerShell interne.

## Technologies utilisées
- **Langage** : C#
- **Framework** : Avalonia 11.2.3
- **PowerShell SDK** : Microsoft.PowerShell.SDK avec PowerShell 7
- **Bibliothèques** :
  - ExcelDataReader (pour lecture de fichiers Excel)
  - LoadingIndicators.Avalonia (indicateur de chargement)

## Architecture du projet
L'application suit une architecture modulaire avec les composants suivants :
- **MainWindow** : Fenêtre principale contenant la navigation et l'affichage des vues.
- **Vues principales** :
  - `Home.axaml.cs` : Gestion de la connexion/déconnexion.
  - `Calendrier.axaml.cs` : Gestion de la visibilité des calendriers.
  - `GestionTeams.axaml.cs` : Gestion des équipes Teams.
  - `Conversations.axaml.cs` : Gestion des conversations et des stratégies de messagerie.
- **Services** :
  - `PowerShellService.cs` : Gestion de l'exécution des commandes PowerShell de manière synchrone et asynchrone.
  - `AccountManager.cs` : Gestion sécurisée des comptes utilisateurs.

## Installation et Exécution
### Prérequis
- .NET 7 ou supérieur
- PowerShell 7
- Modules PowerShell : `Microsoft.Graph.Beta`, `ExchangeOnlineManagement`, `MicrosoftTeams`



