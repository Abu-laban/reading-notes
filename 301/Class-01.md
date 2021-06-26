# Introduction to React and Components

# Component-Based Architecture

The primary objective of component-based architecture is to ensure **component reusability**. A component encapsulates functionality and behaviors of a software element into a reusable and self-deployable binary unit. There are many standard component frameworks such as COM/DCOM, JavaBean, EJB, CORBA, .NET, web services, and grid services.

> Component-oriented software design has many advantages over the traditional object-oriented approaches such as −

> - Reduced time in market and the development cost by reusing existing components.

> - Increased reliability with the reuse of the existing components.

## What is a Component?

_A component is a modular, portable, replaceable, and reusable set of well-defined functionality that encapsulates its implementation and exporting it as a higher-level interface._

## Characteristics of Components

1. `Reusability`

>       Components are usually designed to be reused in different situations in different applications. However, some components may be designed for a specific task.

2. `Replaceable`

>       Components may be freely substituted with other similar components.

3. `Not context specific`

>       Components are designed to operate in different environments and contexts.

4. `Extensible`

>       A component can be extended from existing components to provide new behavior.

5. `Encapsulated`

>        A component depicts the interfaces, which allow the caller to use its functionality, and do not expose details of the internal processes or any internal variables or state.

6. `Independent`

>       Components are designed to have minimal dependencies on other components.

## Advantages

- Ease of deployment

  - As new compatible versions become available, it is easier to replace existing versions with no impact on the other components or the system as a whole.

- Reduced cost

  - The use of third-party components allows you to spread the cost of development and maintenance.

- Ease of development

  - Components implement well-known interfaces to provide defined functionality, allowing development without impacting other parts of the system.

- Reusable

  - The use of reusable components means that they can be used to spread the development and maintenance cost across several applications or systems.

- Modification of technical complexity

  - A component modifies the complexity through the use of a component container and its services.

- Reliability

  - The overall system reliability increases since the reliability of each individual component enhances the reliability of the whole system via reuse.

- System maintenance and evolution

  - Easy to change and update the implementation without affecting the rest of the system.

- Independent
  - Independency and flexible connectivity of components. Independent development of components by different group in parallel. Productivity for the software development and future software development.

# What is “Props” and how to use it in React?

## What is Props?

**React is a component-based library** which divides the UI into little reusable pieces. In some cases, those components need to communicate (send data to each other) and the way to pass data between components is by using **props**.

**“Props”** is a special keyword in React, which stands for **properties** and is being used for **passing data from one component to another**.

> But the important part here is that data with props are being passed in a **uni-directional flow**. (one way from parent to child)

## Using Props in React

1. Firstly, define an attribute and its value(data)
2. Then pass it to child component(s) by using Props
3. Finally, render the Props Data

   **You can also learn how to use Props by watching my tutorial video below:**

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg)](https://www.youtube.com/watch?v=KvapOdsFK5A)

        Props can only be passed to components in one-way (parent to child)


