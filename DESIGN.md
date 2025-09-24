# Project 1 – EC2 REST Converter Design
Ryan Reopell

## Overview
This project is the creation of a REST web service running on an AWS EC2 instance, which converts a user's input in pounds to kilograms. Steps are taken to ensure security

## Stack
*Ubuntu t3.micro on AWS EC2* -- Cloud hosting
*Node.js* -- Runtime environment. Simple and common for roles like this
*Express* -- Node-native routing service
*Morgan* -- Logging

## AWS Hosting
Ubuntu t3.micro, as t2.micro unavailable on free tier
Security group; allow inbound SSH only from personal IP to restrict access, and allow all inbound on 80 and 8080
Create a key pair for more secure access

## Security and Cost hygiene
When finished, delete key pair used, and delete orphaned EBS volumes and/or the instance
