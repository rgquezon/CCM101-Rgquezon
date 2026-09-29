# Multi-Tier Architecture Research

## Two-Tier Architecture Definition
A Two-Tier Architecture is a software design pattern where an application is split into two distinct logical and operational layers: a presentation/application tier and a database tier.

## The Web/Application Tier
The Web/Application Tier is responsible for rendering the user interface, serving static web assets, processing client HTTP requests, executing business logic, and sending backend database queries. In this deployment, the Nextcloud container acts as the Web/Application tier.

## The Database Tier
The Database Tier is dedicated exclusively to storing, managing, and retrieving persistent structured data, user accounts, authentication tokens, file metadata, and system settings. In this deployment, MariaDB acts as the backend database tier.

## Why Separate Web and Database Tiers?
Separating the web server and database into distinct containers improves system security, scalability, and maintainability. It prevents single-point failure vulnerabilities, allows independent scaling of database hardware resources, and enables seamless software updates to the web container without risking database corruption or data loss.
