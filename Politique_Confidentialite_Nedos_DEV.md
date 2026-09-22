# Politique de Confidentialité — Nedos

**Version 1.0 — En vigueur à compter du 9 juin 2026**  
**Dernière mise à jour : 9 juin 2026**

> [SOCIÉTÉ] s'engage à protéger vos données personnelles avec le plus haut niveau de sérieux. Ce document décrit de manière exhaustive et transparente quelles données nous collectons, pourquoi, comment elles sont traitées, où elles sont hébergées, et quels sont vos droits. Nous ne vendons pas vos données. Nous ne les monétisons pas à des fins publicitaires. Point.

---

## Article 1 — Responsable du traitement

**[SOCIÉTÉ]**  
SASU — Capital social : 1 000 euros  
SIRET : [SIRET]  
[ADRESSE]  
Contact délégué : [EMAIL_CONTACT]

[SOCIÉTÉ] est responsable du traitement de vos données personnelles au sens de l'article 4(7) du Règlement Général sur la Protection des Données (RGPD — Règlement UE 2016/679) et de la loi Informatique et Libertés modifiée.

---

## Article 2 — Données collectées et finalités

### 2.1 Données de compte

| Donnée | Finalité | Base légale |
|---|---|---|
| Adresse email | Authentification, communication | Exécution du contrat |
| Mot de passe (haché bcrypt — jamais en clair) | Sécurité du compte | Exécution du contrat |
| Genre, âge, ville | Personnalisation des suggestions de tenues | Exécution du contrat |

### 2.2 Données de garde-robe

| Donnée | Finalité | Base légale |
|---|---|---|
| Photos de vêtements | Affichage, analyse IA des couleurs, génération de tenues | Exécution du contrat |
| Descriptions (catégorie, type, marque, matière, motif) | Suggestions de tenues et analyses | Exécution du contrat |
| Couleurs analysées (nom, valeur hex, référence Pantone) | Moteur de colorimétrie Nedos | Exécution du contrat |
| Saison Nedos
(déclarée manuellement par l'utilisateur) | Personnalisation des analyses et suggestions | Exécution du contrat |

**Important** : la saison Nedos est une préférence stylistique **déclarée librement** par l'utilisateur dans une liste (Printemps, Été, Automne, Hiver). Nedos n'effectue aucune analyse biométrique automatisée de photos du visage ou du corps. Cette donnée ne constitue pas une donnée sensible au sens de l'article 9 du RGPD.

### 2.3 Données d'usage

| Donnée | Finalité | Base légale |
|---|---|---|
| Fonctions utilisées, quotas consommés, horodatages | Gestion des quotas, facturation, prévention des abus | Exécution du contrat / Intérêt légitime |
| Version de l'app, type d'appareil, version iOS | Support technique, compatibilité | Intérêt légitime |

### 2.4 Données que nous ne collectons pas

[SOCIÉTÉ] déclare expressément ne pas collecter :
- Données de géolocalisation précise
- Contacts téléphoniques
- Identifiants publicitaires (IDFA)
- Données de navigation externe à l'application
- Données biométriques au sens de l'article 9 RGPD

---

## Article 3 — Hébergement et localisation des données

### 3.1 Hébergement en Europe — engagement ferme

**L'intégralité des données personnelles des utilisateurs de Nedos est hébergée en République d'Irlande (Union Européenne)**, sur l'infrastructure cloud d'Amazon Web Services (région AWS eu-west-1, Dublin, Irlande), via notre sous-traitant Supabase Inc.

L'Irlande est un État membre de l'Union Européenne. Ce choix d'hébergement garantit que vos données bénéficient de la protection intégrale du RGPD.

[SOCIÉTÉ] s'engage à maintenir cet hébergement en Union Européenne pour la durée de vie du service. Toute modification substantielle de cette localisation fera l'objet d'une information préalable des utilisateurs avec un préavis minimum de 30 jours.

### 3.2 Transferts vers des services d'intelligence artificielle

Nedos utilise des services d'intelligence artificielle tiers dont les serveurs sont situés aux États-Unis. Ces transferts sont strictement encadrés :

**Ce qui est transféré :**
- Les photos de vêtements (jamais de photos de personnes identifiables)
- Les descriptions textuelles des vêtements et tenues

**Ce qui n'est jamais transféré :**
- L'adresse email
- Les données d'identification (nom, prénom)
- Toute donnée permettant d'identifier directement l'utilisateur

**Comment ces transferts sont sécurisés :**
- Les données transitent exclusivement via les serveurs d'[SOCIÉTÉ] (Edge Functions Supabase hébergées en Irlande) — elles ne partent jamais directement depuis l'appareil de l'utilisateur
- Chiffrement en transit TLS 1.2 minimum
- Les données ne sont pas utilisées par les prestataires IA pour entraîner leurs modèles (conformément aux conditions contractuelles applicables)
- Les transferts vers les États-Unis sont encadrés par les Clauses Contractuelles Types (CCT) de la Commission européenne et/ou le Data Privacy Framework UE-États-Unis

| Prestataire IA | Finalité | Localisation | Encadrement du transfert |
|---|---|---|---|
| Anthropic, Inc. (Claude) | Analyse colorimétrique des vêtements, suggestions de tenues | États-Unis | CCT Commission européenne |
| Google LLC (Gemini) | Génération de photos packshot, génération d'images de tenues | États-Unis | CCT Commission européenne / DPF |

---

## Article 4 — Durée de conservation

| Catégorie de données | Durée de conservation |
|---|---|
| Données de compte et garde-robe | Durée d'utilisation active du compte + 30 jours après suppression du compte |
| Photos de vêtements et images générées | Suppression dans les 30 jours suivant la suppression du compte |
| Données d'usage et quotas | 13 mois glissants à compter de l'enregistrement |
| Données de facturation (abonnement Premium) | 10 ans conformément aux obligations comptables légales |

À l'expiration de ces délais, les données sont supprimées de manière définitive et irréversible des systèmes d'[SOCIÉTÉ].

---

## Article 5 — Sécurité des données

[SOCIÉTÉ] met en œuvre les mesures techniques et organisationnelles suivantes pour protéger vos données :

**Mesures techniques :**
- Chiffrement de toutes les communications en transit (HTTPS/TLS 1.2+)
- Stockage des photos et images dans des espaces de stockage privés, inaccessibles publiquement, accessibles uniquement via des URL temporaires signées à durée de vie limitée
- Contrôle d'accès par ligne (Row Level Security — RLS) sur l'intégralité des tables de la base de données : chaque utilisateur ne peut accéder qu'à ses propres données
- Hachage irréversible des mots de passe (bcrypt)
- Authentification par JWT (JSON Web Token) validé côté serveur sur chaque requête
- Clés d'API des services d'intelligence artificielle exclusivement stockées côté serveur, jamais exposées dans le code client ni dans l'application mobile
- Vérification de l'appartenance de chaque ressource à l'utilisateur avant tout traitement (ownership check)
- Timeout et limites de charge sur tous les appels aux services externes

**Mesures organisationnelles :**
- Accès aux données de production strictement limité au personnel technique d'[SOCIÉTÉ]
- Aucune clé secrète ou donnée sensible dans le code source versionné

En cas de violation de données personnelles susceptible d'engendrer un risque pour vos droits et libertés, [SOCIÉTÉ] s'engage à notifier la CNIL dans les 72 heures conformément à l'article 33 du RGPD, et à vous en informer sans délai injustifié si le risque est élevé.

---

## Article 6 — Données anonymisées — traitement conditionnel

Avec votre **consentement explicite et librement donné lors de l'inscription**, [SOCIÉTÉ] peut utiliser des données agrégées et strictement anonymisées (tendances de style, popularité des palettes de couleurs, combinaisons de matières, fréquence d'utilisation des catégories) à des fins d'amélioration du service et d'analyses de marché.

**Garanties :**
- Ces données ne permettent en aucun cas de vous identifier individuellement
- Elles ne sont jamais vendues ni cédées à des tiers sans votre consentement explicite séparé
- Vous pouvez retirer ce consentement à tout moment depuis Paramètres → Confidentialité dans l'application, sans que cela affecte la légalité des traitements effectués avant le retrait

---

## Article 7 — Vos droits (RGPD)

Conformément aux articles 15 à 22 du RGPD et à la loi Informatique et Libertés, vous disposez des droits suivants :

| Droit | Description |
|---|---|
| **Droit d'accès** (art. 15) | Obtenir confirmation que vos données sont traitées et en recevoir une copie complète |
| **Droit de rectification** (art. 16) | Corriger toute donnée inexacte ou incomplète |
| **Droit à l'effacement** (art. 17) | Demander la suppression définitive de vos données ("droit à l'oubli") |
| **Droit à la portabilité** (art. 20) | Recevoir vos données dans un format structuré, couramment utilisé et lisible par machine |
| **Droit d'opposition** (art. 21) | Vous opposer à certains traitements fondés sur l'intérêt légitime |
| **Droit à la limitation** (art. 18) | Demander la suspension temporaire d'un traitement |
| **Droit de retrait du consentement** | Retirer à tout moment votre consentement aux traitements fondés sur celui-ci |

**Pour exercer vos droits :** contactez [SOCIÉTÉ] à [EMAIL_CONTACT] en précisant votre demande et en joignant une copie d'un justificatif d'identité. Nous nous engageons à répondre dans un délai maximum de **30 jours** à compter de la réception de votre demande (délai pouvant être prolongé de 2 mois en cas de demande complexe, avec information préalable).

**Droit de réclamation :** si vous estimez que le traitement de vos données n'est pas conforme au RGPD, vous avez le droit d'introduire une réclamation auprès de la Commission Nationale de l'Informatique et des Libertés (CNIL) :

> **CNIL**  
> 3 place de Fontenoy — TSA 80715 — 75334 Paris Cedex 07  
> www.cnil.fr

---

## Article 8 — Sous-traitants

[SOCIÉTÉ] fait appel aux sous-traitants suivants pour la fourniture du service. Chacun est lié par des obligations contractuelles de confidentialité et de sécurité conformes au RGPD :

| Sous-traitant | Rôle | Localisation des données | Encadrement RGPD |
|---|---|---|---|
| **Supabase Inc.** | Base de données, authentification, stockage fichiers | Irlande, UE (AWS eu-west-1) | DPA conforme RGPD, CCT |
| **Anthropic, Inc.** | Analyse IA des couleurs et tenues (Claude) | États-Unis | CCT Commission européenne |
| **Google LLC** | Génération d'images IA (Gemini) | États-Unis | CCT / Data Privacy Framework |
| **Apple Inc.** | Distribution de l'application, paiements in-app | États-Unis | CCT / Data Privacy Framework |

[SOCIÉTÉ] s'engage à n'avoir recours qu'à des sous-traitants présentant des garanties suffisantes quant à la mise en œuvre de mesures techniques et organisationnelles appropriées.

---

## Article 9 — Cookies et technologies de suivi

L'application mobile Nedos n'utilise **aucun cookie publicitaire, aucun traceur de comportement, aucun SDK analytique tiers**. Des tokens de session techniques (JWT) sont utilisés exclusivement pour maintenir votre authentification. Ces tokens sont nécessaires au fonctionnement du service et ne peuvent pas être désactivés.

---

## Article 10 — Mineurs

Nedos est destinée aux personnes âgées de 16 ans ou plus conformément à l'article 8 du RGPD et à la loi française. [SOCIÉTÉ] ne collecte pas sciemment de données personnelles de personnes de moins de 16 ans. Si un parent ou tuteur légal constate qu'un mineur de moins de 16 ans a créé un compte, il peut en demander la suppression immédiate à [EMAIL_CONTACT]. [SOCIÉTÉ] procédera à la suppression dans les meilleurs délais.

---

## Article 11 — Modifications de la politique de confidentialité

[SOCIÉTÉ] se réserve le droit de modifier la présente politique à tout moment pour refléter des évolutions légales, réglementaires ou techniques. En cas de modification substantielle affectant vos droits, vous serez informé par notification dans l'application ou par email avec un préavis minimum de 30 jours. La date de dernière mise à jour est indiquée en tête du document. La poursuite de l'utilisation de l'application après ce délai vaut acceptation des modifications.

---

## Article 12 — Contact et réclamations

Pour toute question relative à la présente politique ou pour exercer vos droits :

**[SOCIÉTÉ] — Délégué à la protection des données**  
[ADRESSE]  
[EMAIL_CONTACT]  
*(Délai de réponse : 30 jours maximum)*

> **Note** : Cette politique de confidentialité a été rédigée avec le plus grand soin. [SOCIÉTÉ] recommande sa validation par un avocat spécialisé en droit du numérique et en droit de la protection des données avant toute mise en production ou soumission à l'App Store.
