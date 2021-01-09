# Introduction

Welcome to Zero to IoT! This book will take you through designing/building your own prototype "Internet Of Things" board, writing firmware for it, and then designing software that runs in the cloud to aggregate data from said board(s)!

We are going to take a wild ride together. There will be tears, there will be laughter, there will hopefully be some learning for learning's sake.

We will mostly be using the Rust Programming Language to program our IoT board, as well as our application that will collect information from our board.

I don't need to convince you of the benefits of using this language. If we can set it up, we can use it for ALL of our work! Sounds great because it is.

> This book assumes no prior Rust experience. However, does assume you have _some_ programming experience. As there exists _tons_ of Rust documentation, I will link out to existing sources for relevant information.

## The Plan

We will build a board that has GPS, an Accelerometer, and an LTE capable processor. We will also add an I2C QT Stemma connector so we can attach another sensor board. With this setup we can use the Accelerometer to wake up our processor and send information, including GPS coordinates, to the cloud.

## Technologies & Tools Covered

* [RustLang](https://rust-lang.org) - Rust Programming Language
* [EasyEDA](https://easyeda.com/) - Schematic and PCB Design
* [GitHub](https://github.com) - Code Repository
* [Docker](https://www.docker.com/) - Containers
* [Kubernetes](https://kubernetes.io/) - Deploying Containers
* Cloud Services
    * [AWS](https://aws.amazon.com/) - Amazon Cloud Web Services
    * [GCP](https://cloud.google.com/) - Google Cloud Web Services
    * [Digital Ocean](https://www.digitalocean.com/) - Digital Ocean Cloud Web Services
* Electrical Components
    * GPS
    * Accelerometer
    * LTE

## How to read this book

This book starts with electricity fundamentals and basic circuits. Works its way into the hardware world, then quickly comes firmware (software that runs directly on hardware). After our IoT board is sending data to the cloud, we will cover basic web application fundamentals. We will build a web app and deploy it to a cloud provider of your choosing. The application will store information in a database that we set up as part of this process. Each section should be able to stand on it's own and be perused independently of each other. Feel free to skip sections depending on how and what understanding you may already have.

> Note that I do not claim to be an expert in EVERY area we cover. I will do my best to say everything we build will be worthy of a "Prototype" title.

TLDR;
Book reads from Sensor to Cloud, top to bottom.

## Styling conventions

> ### Command Line Notation
>
> In this chapter and throughout the book, we’ll show some commands used in the
> terminal. Lines that you should enter in a terminal all start with `$`. You
> don’t need to type in the `$` character; it indicates the start of each
> command. Lines that don’t start with `$` typically show the output of the
> previous command. Additionally, Windows-specific examples will use `>`
> rather than `$`.

## Resources

Some excellent resources that we will constantly link to:

* [Rust Book](https://doc.rust-lang.org/stable/book/)
* [Rust Embedded Book](https://docs.rust-embedded.org/book/)
* [Rust Embedded Discovery Book](https://docs.rust-embedded.org/discovery/)