---
title: "Setup Analligence Chrome Ghost"
---

# Analligence Chrome Ghost javascript injecting module

## Introduction

Chrome Ghost is an extension for chrome web browser where you can inject Analligence script to verify everything working fine before pushing it to your environment.

## Usage

Download latest release from [Analligence Chrome Ghost Release](https://github.com/next-time-space/analligence-chrome-ghost/releases)

1. Click on Drag downloaded crx file to Chrome to install
2. Click on extension `Analligence Chrome Ghost` from extension bar -> Enable it first
3. Click on `Options`
4. Enter host name. If your host starts with `www.` provide that too. Multiple host can be given by comma separated.
5. Select Javascript file or proivide URL to inject on the page.
6. Save.
7. Go to the target page. Check console logs. It should print `Analligence Script loaded.`