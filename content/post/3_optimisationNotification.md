+++
title = 'Comment faire un système de notifications scalable?'
date = 2024-01-20
author = "quinteirosm"
keywords = ["notification", "webhooks", "scalability" ]
cover = ""
summary = "Razorpay, une plateforme de paiement innovante, a récemment amélioré son système de notification pour gérer efficacement les communications avec ses clients. Cet article explore les défis auxquels Razorpay était confronté, les solutions mises en œuvre, et comment l'entreprise a assuré l'observabilité de son système."
+++

# Comment Razorpay a optimisé son système de notification avec les webhooks et Kinesis

## Introduction

Razorpay, une plateforme de paiement innovante, a récemment amélioré son système de notification pour gérer efficacement les communications avec ses clients. Cet article explore les défis auxquels Razorpay était confronté, les solutions mises en œuvre, et comment l'entreprise a assuré l'observabilité de son système.

## Qu'est-ce qu'un webhook?

Un **webhook** est un moyen pour une application d'envoyer des informations en temps réel à d'autres applications. Il fonctionne comme un signal envoyé à une URL prédéfinie en réponse à des événements spécifiques dans la source. Cela permet une intégration et une réactivité système à système.

## Problèmes de performance de la base de données

Razorpay a rencontré des problèmes de performance avec sa base de données lors de la montée en charge de son service de notification. Avec l'augmentation du volume de transactions, la base de données a été surchargée, entraînant des retards et des échecs dans l'envoi des notifications.

## L'utilisation de Kinesis pour la mise à l'échelle

Pour surmonter ces défis, Razorpay a intégré **Amazon Kinesis**, un service de streaming de données en temps réel. Kinesis a permis à Razorpay de collecter, traiter et analyser des flux de données en temps réel, offrant ainsi une solution évolutive pour gérer les pics de charge sans compromettre les performances.

## Gestion des réponses retardées des clients

Les réponses tardives des clients aux notifications peuvent entraîner des files d'attente et affecter le temps de traitement. Razorpay a résolu ce problème en mettant en œuvre un système de nouvelle tentative intelligent qui ajuste dynamiquement les délais entre les tentatives en fonction du comportement du client.

## Assurer l'observabilité du système

Pour maintenir la fiabilité et la transparence, Razorpay a mis en place un cadre d'observabilité complet. Cela comprend le suivi des performances, la journalisation des événements et la mise en place d'alertes pour surveiller l'état du système de notification en temps réel.

## Conclusion

L'évolution du système de notification de Razorpay illustre l'importance d'une infrastructure évolutive et réactive pour gérer les communications client. En utilisant des webhooks et Amazon Kinesis, Razorpay a non seulement résolu ses problèmes initiaux mais a également posé les bases pour une croissance future sans entraves.

## En quoi cela m'est utile

Cet article m'a intéressé car nous sommes actuellement entrain de développer une application mobile hybride pour un cours à la HEIG-VD et on nous a demandé d'utiliser des fonctions natives à l'OS dont fait partie le système de notifications. Je souhaitais donc savoir comment optimiser au possible cet aspect de l'application. Au final je ne l'ai pas utilisé car, à notre échelle, cela ne faisait pas de sens de se compliquer la vie avec un système plus optimisé mais aussi plus complexe.

## Source

[https://blog.quastor.org/](https://blog.quastor.org/p/build-scalable-notification-service)
