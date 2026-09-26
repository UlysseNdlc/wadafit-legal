# Politique de confidentialité — Nedos

**Version 2.0 — En vigueur à compter du 26/09/2026**
**Dernière mise à jour : 26/09/2026**

> Ce document explique quelles données Nedos traite, pourquoi, avec qui elles sont partagées, combien de temps elles sont conservées et quels sont vos droits. Nous ne vendons pas vos données personnelles. Avec l'offre gratuite, et seulement avec votre consentement, vos données de garde-robe peuvent être exploitées sous forme de statistiques anonymisées, y compris à des fins publicitaires (article 6).

---

## Article 1 — Responsable du traitement

**ODY SERVICES SASU**
Société par actions simplifiée à associé unique — capital social : 1 000 euros
RCS Paris 944 378 249 — SIRET 944 378 249 00014
Siège : 61 rue de Lyon, 75012 Paris
Contact pour toute question relative à vos données : contact@nedos.app

ODY SERVICES est responsable du traitement de vos données personnelles au sens de l'article 4(7) du Règlement général sur la protection des données (RGPD — Règlement UE 2016/679) et de la loi Informatique et Libertés modifiée. Elle n'a pas désigné de délégué à la protection des données ; l'adresse ci-dessus est le point de contact unique.

---

## Article 2 — Données traitées et finalités

### 2.1 Données de compte

| Donnée | Finalité | Base légale |
|---|---|---|
| Adresse e-mail | Création du compte, connexion, e-mails de service (confirmation d'inscription, réinitialisation du mot de passe, suppression du compte) | Exécution du contrat |
| Mot de passe (stocké uniquement sous forme hachée, jamais en clair) | Sécurité du compte | Exécution du contrat |
| Nom et prénom | Personnalisation de l'affichage | Exécution du contrat |
| Clé de double authentification (si vous activez l'authentification à deux facteurs) | Sécurité du compte | Exécution du contrat |
| Choix exprimés à l'inscription (acceptation des CGU et de la présente politique, consentement de l'article 6) et leur date | Preuve de l'acceptation et du consentement | Obligation légale (art. 7(1) RGPD) / intérêt légitime |

### 2.2 Données de profil (facultatives)

| Donnée | Finalité | Base légale |
|---|---|---|
| Genre | Adapter les catégories de vêtements et les suggestions | Exécution du contrat |
| Année de naissance | Adapter l'âge apparent du mannequin des images de tenues | Exécution du contrat |
| Ville | Météo locale (accueil, tenue du jour, suggestions adaptées à la météo) | Exécution du contrat |
| Teint et sous-ton de peau, choisis par vous dans une palette | Calcul de votre palette de couleurs et teint du mannequin des images de tenues | Exécution du contrat |
| Silhouette (morphologie), choisie par vous dans une liste | Silhouette du mannequin des images de tenues | Exécution du contrat |
| Photo de portrait | Affichage dans votre profil | Exécution du contrat |
| Préférences (météo, notification de la tenue du jour) | Fonctionnement de ces options | Exécution du contrat |

**Important** : le teint, le sous-ton et la silhouette sont **déclarés par vous**, en choisissant dans une liste. Nedos n'analyse aucune photo de votre visage ou de votre corps ; votre photo de portrait n'est jamais transmise à un service d'intelligence artificielle. Votre palette de couleurs est calculée sur votre appareil à partir de ces choix. Toutes ces données sont facultatives : vous pouvez utiliser Nedos sans les renseigner et les modifier ou les effacer à tout moment depuis votre profil.

### 2.3 Données de garde-robe et de tenues

| Donnée | Finalité | Base légale |
|---|---|---|
| Photos de vêtements | Affichage, détourage (photo « packshot »), analyse des couleurs, génération d'images de tenues | Exécution du contrat |
| Caractéristiques des vêtements (catégorie, type, marque, matière, motif, nom) | Suggestions de tenues | Exécution du contrat |
| Couleurs analysées (nom, valeur hexadécimale, référence Pantone) | Moteur de colorimétrie | Exécution du contrat |
| Tenues enregistrées et images de tenues générées | Consultation, partage à votre initiative | Exécution du contrat |

Nedos ne vous demande jamais de photographier une personne. Nous vous recommandons de photographier vos vêtements seuls, sans personne identifiable.

### 2.4 Données d'usage

| Donnée | Finalité | Base légale |
|---|---|---|
| Journal des appels aux fonctions d'intelligence artificielle (fonction utilisée, succès ou échec, date et heure) | Calcul des quotas d'utilisation, prévention des abus | Exécution du contrat / intérêt légitime |
| Journaux techniques de nos prestataires d'hébergement (dont adresse IP, date et heure des requêtes) | Sécurité, diagnostic des incidents | Intérêt légitime |
| Jeton de notification de l'appareil (uniquement si vous autorisez les notifications) | Envoi des notifications | Exécution du contrat |

### 2.5 Données que nous ne collectons pas

Nedos ne collecte pas : votre géolocalisation (seule la ville que vous saisissez est utilisée), vos contacts, votre identifiant publicitaire (IDFA), votre navigation en dehors de l'application, ni aucune donnée biométrique. L'application n'intègre aucun outil de mesure d'audience ni aucun traceur publicitaire.

---

## Article 3 — Hébergement

Votre compte, vos données de profil, de garde-robe et de tenues ainsi que vos photos sont hébergés par notre prestataire Supabase, dans la région eu-west-1 (Irlande), au sein de l'Union européenne.

Les traitements côté serveur (appels aux services d'intelligence artificielle, suppression de compte) sont exécutés par les fonctions serveur de Supabase, qui s'exécutent dans la région de l'infrastructure la plus proche de l'utilisateur. Vos photos et vos données ne sont jamais envoyées directement depuis votre appareil aux services d'intelligence artificielle : elles passent toujours par ces fonctions, qui contrôlent votre identité et votre quota. Aucune clé d'accès à ces services n'est présente dans l'application.

---

## Article 4 — Destinataires et transferts hors de l'Union européenne

### 4.1 Services d'intelligence artificielle

| Prestataire | Ce qui lui est transmis | Finalité | Localisation | Encadrement du transfert |
|---|---|---|---|---|
| **Anthropic, PBC** (Claude) | Photos de vêtements ; caractéristiques des vêtements ; genre ; ville et météo du jour si l'option météo est activée | Analyse des couleurs, suggestions de tenues | États-Unis | Clauses contractuelles types de la Commission européenne (accord de traitement des données d'Anthropic) |
| **Google LLC** (Gemini) | Photos et caractéristiques des vêtements ; genre ; âge approximatif (calculé à partir de l'année de naissance) ; silhouette ; teint et sous-ton | Détourage des photos de vêtements, génération des images de tenues (mannequin sans visage) | États-Unis | Cadre de protection des données UE–États-Unis (Data Privacy Framework) et clauses contractuelles types |

**Ne sont jamais transmis à ces prestataires** : votre adresse e-mail, votre nom, votre photo de portrait, ni aucun identifiant de compte.

Ces prestataires n'utilisent pas les données que nous leur transmettons pour entraîner leurs modèles, conformément à leurs conditions applicables aux services professionnels. Ils peuvent les conserver pour une durée limitée afin de détecter les abus, selon leurs propres conditions.

### 4.2 Autres prestataires et destinataires

| Destinataire | Rôle | Données concernées | Localisation |
|---|---|---|---|
| **Supabase, Inc.** | Base de données, authentification, stockage des fichiers, fonctions serveur (sous-traitant) | Toutes les données décrites à l'article 2 | Union européenne (Irlande) — société établie aux États-Unis |
| **Resend** | Envoi des e-mails de service (sous-traitant) | Adresse e-mail, contenu de l'e-mail | Union européenne (région eu-west-1) — société établie aux États-Unis |
| **OpenMeteo GmbH** | Service météo, interrogé directement par votre appareil (responsable de traitement indépendant) | Nom de la ville saisie ; votre adresse IP, comme pour toute requête internet (journaux conservés 90 jours par Open-Meteo) | Suisse (pays reconnu par la Commission européenne comme offrant un niveau de protection adéquat) |
| **Apple Inc.** | Distribution de l'application, paiement de l'abonnement Premium (responsable de traitement indépendant) | Données d'achat, selon la politique de confidentialité d'Apple | Selon Apple |

Nos sous-traitants sont liés par des engagements contractuels conformes à l'article 28 du RGPD. Lorsqu'une société est établie hors de l'Union européenne, l'accès éventuel à vos données depuis l'étranger est encadré par les clauses contractuelles types de la Commission européenne ou par le cadre de protection des données UE–États-Unis (Data Privacy Framework).

---

## Article 5 — Durées de conservation

| Catégorie de données | Durée de conservation |
|---|---|
| Données de compte, de profil, de garde-robe, de tenues et photos | Tant que votre compte est actif. Un compte sans aucune connexion pendant 3 ans est supprimé, après un e-mail d'avertissement envoyé au moins 30 jours avant. |
| Toutes ces données après une demande de suppression du compte | 15 jours (délai d'annulation, voir article 7), puis effacement définitif au plus tard le lendemain |
| Journal des appels aux fonctions d'intelligence artificielle | 13 mois, et dans tous les cas effacé avec le compte |
| Preuve de votre consentement (article 6) et de l'acceptation des CGU | Pendant toute la durée du compte |
| Journaux techniques de l'hébergeur | 7 jours |
| Sauvegardes quotidiennes de la base de données | 7 jours (elles ne contiennent pas les photos) |
| Journaux d'envoi des e-mails de service | 30 jours au plus, chez notre prestataire d'envoi |
| Données transmises aux services d'intelligence artificielle | Durée limitée fixée par chaque prestataire (article 4.1) |
| Données d'achat de l'abonnement | Conservées par Apple, selon sa politique. Les relevés de vente qu'Apple nous transmet ne permettent pas d'identifier les acheteurs ; ils sont conservés 10 ans au titre de nos obligations comptables |
| Statistiques anonymisées (article 6) | Sans limitation : elles ne permettent plus de vous identifier et ne sont plus des données personnelles |

À l'expiration de ces durées, les données sont effacées définitivement ou rendues anonymes.

---

## Article 6 — Offre gratuite et consentement au partage de données anonymisées (« Pay or Okay »)

### 6.1 Le principe

Nedos est proposée sous deux formules, au choix de l'utilisateur :

- **l'offre gratuite**, dont l'accès est subordonné à votre consentement au traitement décrit ci-dessous ;
- **l'offre Premium**, payante, qui donne accès au service sans ce consentement.

Vous avez donc toujours le choix entre consentir et utiliser l'offre gratuite, ou refuser et souscrire l'offre Premium. Ce modèle, dit « Pay or Okay », est encadré par les lignes directrices du Comité européen de la protection des données.

### 6.2 Ce à quoi vous consentez

ODY SERVICES peut exploiter vos données de garde-robe et de profil (catégories, marques, matières, motifs et couleurs de vos vêtements, tenues composées, palettes de couleurs, genre, tranche d'âge, ville) pour produire des **statistiques agrégées et anonymisées** — tendances de style, popularité des couleurs, des matières ou des marques — utilisées :

- pour améliorer Nedos ;
- pour réaliser et commercialiser, auprès de marques, d'annonceurs ou d'autres partenaires, des études et statistiques de tendances, qui peuvent servir à des campagnes publicitaires diffusées dans Nedos ou en dehors de Nedos.

Seules des statistiques agrégées, qui ne permettent pas d'identifier un utilisateur, peuvent sortir de Nedos. **Aucune donnée personnelle identifiable n'est vendue, louée ou cédée**, et les marques et annonceurs n'ont jamais accès à vos données individuelles. Vos photos, votre adresse e-mail, votre nom et votre portrait ne sont jamais utilisés pour ces statistiques. À la date de la présente version, aucune statistique n'a encore été commercialisée.

**Publicité personnalisée dans l'application** : si Nedos affiche un jour des contenus sponsorisés choisis en fonction de votre garde-robe ou de votre profil (par exemple une pièce de marque suggérée pour compléter votre vestiaire), ce ciblage constituera un traitement de vos données personnelles distinct des statistiques anonymisées. Il sera décrit dans une mise à jour de la présente politique et votre consentement spécifique vous sera demandé avant sa mise en œuvre.

**Base légale** : votre consentement (article 6(1)(a) du RGPD).

### 6.3 Recueil du consentement

Le consentement est recueilli à l'inscription par une case à cocher distincte de l'acceptation des CGU et de la présente politique. Sa date est enregistrée.

### 6.4 Retrait du consentement

Vous pouvez retirer votre consentement à tout moment :

- **si vous êtes abonné Premium**, depuis votre profil, option « Partager mes données anonymisées » ;
- **si vous utilisez l'offre gratuite**, en souscrivant l'offre Premium puis en désactivant l'option, ou en supprimant votre compte (article 7).

Le retrait ne remet pas en cause les traitements effectués auparavant. Les statistiques déjà produites, étant anonymes, ne peuvent plus être rattachées à vous et ne sont pas supprimées.

**Si votre abonnement Premium prend fin**, vous repassez à l'offre gratuite et à ses conditions. Si vous aviez retiré votre consentement, il vous est redemandé ; il n'est jamais rétabli sans votre accord. Tant que vous ne l'avez pas donné, les fonctionnalités de l'offre gratuite ne vous sont pas accessibles ; vous pouvez à tout moment vous réabonner, exporter votre garde-robe ou supprimer votre compte.

---

## Article 7 — Suppression de votre compte

Vous pouvez supprimer votre compte à tout moment depuis l'application : **Profil → Paramètres (roue dentée) → Supprimer mon compte**, après avoir saisi à nouveau votre mot de passe.

- **Désactivation immédiate** : dès la demande, votre compte est désactivé et vos sessions ouvertes sont fermées sur tous vos appareils. Vos données ne sont plus accessibles et ne sont plus transmises à aucun service d'intelligence artificielle.
- **Délai d'annulation de 15 jours** : un e-mail de confirmation vous est envoyé. Pendant 15 jours, vous pouvez annuler la suppression en vous reconnectant et en choisissant « Réactiver mon compte ». Pendant ce délai, votre adresse e-mail ne peut pas être utilisée pour créer un nouveau compte.
- **Effacement définitif** : à l'issue des 15 jours, votre compte et l'ensemble de vos données — profil, garde-robe, tenues, journal d'utilisation, ainsi que toutes vos photos et images (vêtements, tenues, portrait) — sont effacés définitivement, au plus tard le lendemain. Cet effacement est irréversible. Les sauvegardes quotidiennes de la base de données, conservées 7 jours, peuvent encore contenir vos données pendant cette durée ; elles ne contiennent pas vos photos, qui sont effacées immédiatement.
- **Abonnement Premium** : supprimer votre compte **ne résilie pas** votre abonnement, qui est géré par Apple. Résiliez-le dans les réglages de votre appareil (Réglages → [votre nom] → Abonnements) pour ne plus être facturé. La période en cours n'est pas remboursée par ODY SERVICES ; les demandes de remboursement relèvent d'Apple.

Vous pouvez aussi demander la suppression de votre compte par e-mail à contact@nedos.app.

---

## Article 8 — Sécurité

Mesures techniques :
- chiffrement de toutes les communications (HTTPS/TLS) ;
- photos et images stockées dans des espaces privés, accessibles uniquement par des liens temporaires signés ;
- contrôle d'accès par ligne (Row Level Security) sur toutes les tables contenant des données d'utilisateurs : chaque utilisateur n'accède qu'à ses propres données ;
- mots de passe stockés uniquement sous forme hachée ;
- authentification à deux facteurs (TOTP) disponible pour tous, appliquée côté serveur lorsqu'elle est activée ;
- vérification de l'identité et du quota de l'utilisateur, côté serveur, avant tout appel à un service d'intelligence artificielle ;
- clés d'accès aux services d'intelligence artificielle conservées exclusivement côté serveur.

Mesures organisationnelles : accès aux données de production limité aux seules personnes qui en ont besoin ; aucune clé secrète dans le code source.

En cas de violation de données personnelles présentant un risque pour vos droits et libertés, ODY SERVICES la notifie à la CNIL dans les 72 heures (article 33 du RGPD) et vous en informe dans les meilleurs délais si le risque est élevé (article 34).

---

## Article 9 — Vos droits

Conformément aux articles 15 à 22 du RGPD, vous disposez des droits suivants :

| Droit | Description |
|---|---|
| **Accès** (art. 15) | Savoir si vos données sont traitées et en obtenir une copie |
| **Rectification** (art. 16) | Corriger des données inexactes — la plupart se modifient directement dans l'application |
| **Effacement** (art. 17) | Faire supprimer vos données — directement depuis l'application (article 7) |
| **Limitation** (art. 18) | Faire suspendre temporairement un traitement |
| **Portabilité** (art. 20) | Recevoir les données que vous nous avez fournies dans un format structuré et lisible par machine |
| **Opposition** (art. 21) | Vous opposer aux traitements fondés sur notre intérêt légitime |
| **Retrait du consentement** (art. 7(3)) | Voir article 6.4 |
| **Directives post-mortem** (loi Informatique et Libertés, art. 85) | Définir le sort de vos données après votre décès |

**Pour exercer vos droits** : écrivez à contact@nedos.app depuis l'adresse associée à votre compte. Nous pourrons vous demander un justificatif d'identité uniquement en cas de doute raisonnable sur votre identité. Nous répondons dans un délai d'un mois, prolongeable de deux mois pour les demandes complexes, auquel cas nous vous en informons.

**Réclamation** : vous pouvez introduire une réclamation auprès de la CNIL — 3 place de Fontenoy, TSA 80715, 75334 Paris Cedex 07 — www.cnil.fr.

---

## Article 10 — Traceurs

L'application n'utilise aucun cookie ni traceur publicitaire ou de mesure d'audience. Elle conserve sur votre appareil uniquement ce qui est nécessaire à son fonctionnement : votre session de connexion et quelques préférences d'affichage (par exemple la tenue du jour choisie). Ces éléments sont strictement nécessaires au service et ne requièrent pas de consentement.

---

## Article 11 — Mineurs

Nedos est réservée aux personnes âgées d'au moins 16 ans. Nous ne collectons pas sciemment de données concernant des personnes de moins de 16 ans. Un parent ou tuteur qui constate qu'un mineur de moins de 16 ans a créé un compte peut en demander la suppression à contact@nedos.app ; elle est alors effectuée sans délai d'annulation.

---

## Article 12 — Modifications

Nous pouvons modifier la présente politique pour tenir compte d'évolutions légales, réglementaires, techniques ou du service. En cas de modification substantielle, vous en êtes informé dans l'application ou par e-mail au moins 30 jours à l'avance. Si une modification porte sur un traitement fondé sur votre consentement, votre consentement vous sera à nouveau demandé. La date de dernière mise à jour figure en tête du document.

---

## Article 13 — Contact

**ODY SERVICES SASU**
61 rue de Lyon, 75012 Paris
contact@nedos.app
