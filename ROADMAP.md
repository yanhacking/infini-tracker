# INFINI — Roadmap du projet

Suivi de l'avancement de la plateforme e-commerce INFINI (bougies de luxe, édition Or Massif).
Chaque case cochée correspond à une fonctionnalité réellement construite et vérifiée.

## 🏗️ PHASE 0 — Fondations

- [x] Schéma de base de données complet (25+ tables : produits, commandes, comptes, CMS, sécurité)
- [x] API REST PHP versionnée (/api/v1)
- [x] Connexion du frontend cinématique existant à l'API réelle
- [x] Middlewares de sécurité (CORS, en-têtes HTTP, limitation des tentatives de connexion)

## 🎨 PHASE 1 — CMS complet (zéro contenu codé en dur)

- [x] Panel admin avec authentification sécurisée (rôles, CSRF, rate limiting)
- [x] Éditeur de pages en blocs (texte / image / vidéo) — Accueil, À propos, Contact, FAQ, Livraison, Retours, Mentions légales, Confidentialité
- [x] Réglages globaux éditables (nom de marque, tagline, manifeste)
- [x] Bibliothèque média avec optimisation automatique (redimensionnement, compression, conversion WebP)
- [x] Gestion des produits + upload photos/vidéos depuis l'admin
- [x] Chapitres vidéo de la page d'accueil 100% éditables (vidéo, photo de secours, mise en page, produit lié)
- [x] Journal d'activité admin (audit de chaque action)

## 🛒 PHASE 2 — Achat complet

- [x] Authentification client (inscription / connexion / tokens de session)
- [x] Dashboard client (historique et statut des commandes)
- [x] Création de commande sécurisée (prix et stock revalidés côté serveur, jamais confiés au front)
- [x] Intégration Stripe (Payment Intent + webhook signé)
- [x] Intégration PayPal (Orders API v2 + capture + webhook)
- [x] Intégration Goshippo (tous les tarifs transporteurs affichés au client + achat automatique de l'étiquette)
- [x] Décrément automatique du stock + historique de statut de commande
- [x] Emails transactionnels automatiques (confirmation de compte, commande, paiement, expédition, mot de passe oublié)

## 🕯️ PHASE 3 — Catalogue avancé

- [x] Variantes produits (tailles, éditions limitées)
- [x] Catégories produits
- [x] Moteur de recherche (nom, description, parfum)
- [x] Avis clients + modération admin
- [x] Liste de souhaits (wishlist)

## 📣 PHASE 4 — Marketing

- [ ] Codes promo / coupons (pourcentage, montant fixe, livraison offerte)
- [ ] Newsletter (inscription, confirmation, désinscription, export)
- [ ] Notifications admin en temps réel (nouvelle commande, stock faible, nouveau client)

## 📊 PHASE 5 — Data & mise à l'échelle

- [ ] Dashboard analytics avancé (chiffre d'affaires, panier moyen, taux de conversion)
- [ ] Statistiques internes (vues produits, ajouts panier, abandons de panier)
- [ ] SEO avancé (meta, Open Graph, Twitter Card, Schema.org)
- [ ] Revue de sécurité finale avant mise en production
- [ ] Sauvegardes automatiques avec rotation (base de données + médias)
