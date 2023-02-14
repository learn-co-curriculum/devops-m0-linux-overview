# Introduction to Linux and Operating Systems

## Learning goals

- Understand the basics of operating systems
  - CPU, RAM, Storage
  - Kernel vs Operating System
- Start becoming acquainted with *Linux* operating systems
  - History
  - Why use it?

## Introduction

All around us, we rely on computers to communicate, work, and access information. Centered at the heart of this technology are operating systems, which among other things, manage the hardware and software resources of a computer. In this lesson, we will be exploring the basics of operating systems, as well as introducing one of the most popular operating systems around: *Linux*.

## Operating systems

The most important piece of software (or collection of software) that runs on your computer is the *operating system*.

The **operating system** is primarily responsible for *coordinating* the usage between the hardware (*CPU*, *RAM*, *Storage*, etc.) and the software running on that computer, as well as other functions like scheduling tasks, allocating memory, etc. Here's a very brief breakdown of some the hardware components:

- **CPU** (Central Processing Unit): Executes the instructions that make up a program; performs primarily arithmetic and I/O operations.
- **RAM** (Random-Access Memory): Memory that can be read/written in any order, meaning it is *very* fast. The trade-off is smaller amounts of memory than standard storage. Used for temporary data (program data, machine code, etc) since it is cleared very often. Also referred to as *primary storage*.
- **Storage** (Hard/Solid-state Drives): This type of storage is cheaper and larger in size, while also being non-volatile and retaining data between reboots. Used for persistent data (system files, user files, etc). Also referred to as *secondary storage*.

The most crucial part of the operating system is what is known as the *kernel*.

The **kernel** is a very *low-level* program that sits at the core of the operating system, having *near-complete* control over the entire operating system. It is concerned with handling interactions between the hardware and the software, including device drivers, resource usage, networking, etc. The kernel is typically the first program loaded after the *bootloader*, which handles the initial booting of the system.

The remaining part of the operating system is commonly referred to as *user space* or *userland*. **User space** refers to essentially all code running *outside* of the kernel (but can still interact with it). This includes everything from init systems (responsible for starting up the OS), window managers (drawing windows to the screen, maximize/minimize functionality, etc.), to applications like your web browser.

![User-space vs Kernel-space](https://curriculum-content.s3.amazonaws.com/6685/devops-m0-linux-overview/userspace-vs-kernelspace.png)

You are most likely already familiar with the most popular PC operating systems: **Windows**, **MacOS**, and **Linux**.

This course focuses on *Linux*, for reasons which will become apparent very soon.

## Linux and GNU

**Linux** is an operating system created by *Linus Torvalds* in 1991. He came up with the idea when he had suggestions for another popular family of operating systems known as **UNIX**, and had his ideas rejected. 

*Linux*, in reality, is actually a *kernel* and not a full operating system. When you hear of *Linux* referred to in the context of an operating system, what is usually referred to is a Linux-derivative operating system, or **distro**, of which there are many. 

Here's an infographic showcasing what the market share distribution of *Linux* server distros looks like:

![Linux distro marketshare](https://curriculum-content.s3.amazonaws.com/6685/devops-m0-linux-overview/linux-distros.png)

> Note: These are only *Linux servers*, the marketshare for *Linux desktop* would look different

Linus went ahead and made his creation completely free and open-source, in contrast to *UNIX*. This had the advantage that programmers everywhere could use *Linux* to design their own custom operating systems, including the aforementioned distros, as well as other operating systems, like *Android*.

Even then, however, *Linux* needed more than just the kernel if it wanted to succeed. That's where the *GNU* project came in.

**GNU** is a comprehensive collection of free and open-source software/tools typically used together with Linux. GNU stands for *GNU'S Not UNIX!*, an acronym chosen due to its similarities with *UNIX*, yet differing in the fact that it is free and in actuality contains no *UNIX* code. We will learn these tools intimately in the upcoming chapters.

There are many reasons to use *GNU/Linux*, some of which including:

- No cost
- Relatively simple to become proficient in
- Well-suported software ecosystem, with many industry-grade tools being available for free
- Open source nature means that *anyone* with programming experience and the time can make fixes or additions
- Safety model is consistent and easy to understand
- Lightweight, using minimal computer resources and booting quickly

As a result, *Linux* has quickly become the most used operating system for many applications, such as online servers and embedded systems. If you're wondering what type of operating system is hosting a website, the answer most of the time is *Linux*.

## Conclusion

Operating systems are an essential part of modern technology, managing and organizing the resources used by computers. While this general overview isn't the most comprehensive, you'll quickly come to appreciate all the inner-workings of *Linux* and operating systems as we dive deeper into how all these aspects come together later on.
