# Producer-Consumer Problem Multi-Threading Project

This project demonstrates the implementation of the classic Producer-Consumer problem using Java's multi-threading capabilities. The Producer-Consumer problem is a common synchronization challenge in computer science, where multiple producer threads generate data and multiple consumer threads consume the generated data, while ensuring safe and efficient access to a shared buffer.

## Introduction

The Producer-Consumer problem serves as an example of thread synchronization and inter-process communication. In this project, we explore how to efficiently manage the interactions between producers and consumers using Java's `Thread` class and synchronization constructs.

## Problem Statement

The problem involves a shared buffer between producer threads and consumer threads. Producers generate data items and place them in the buffer, while consumers retrieve and process these items from the buffer. The challenge lies in preventing race conditions, ensuring that producers do not insert data into a full buffer, and consumers do not extract data from an empty buffer.

## Project Highlights

- **Java Multi-Threading**: This project utilizes Java's built-in `Thread` class to implement both producer and consumer threads, showcasing how multi-threading can be effectively utilized.

- **Thread Synchronization**: To ensure proper synchronization and avoid race conditions, the project employs techniques like `synchronized` methods or blocks, `wait`, and `notify` mechanisms.

- **Shared Buffer**: The shared buffer is implemented using data structures like arrays or queues, demonstrating the safe access and management of shared resources among threads.

## Implementation Details

- **Producer**: The producer thread generates data items and adds them to the shared buffer. If the buffer is full, the producer waits until space is available.

- **Consumer**: The consumer thread retrieves data items from the buffer and processes them. If the buffer is empty, the consumer waits until items are available.

- **Synchronization**: Proper synchronization is achieved using the `synchronized` keyword to ensure that only one thread can access critical sections at a time. Additionally, `wait` and `notify` mechanisms are used for efficient thread communication.

## Requirements

- Java JDK 8 or higher
