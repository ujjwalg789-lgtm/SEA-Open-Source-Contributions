# Online Canteen Food-Ordering System

**Name:** Ujjwal Gupta
**USN:** NB25CSE392
**Assigned Case Study:** Question 2 – Mobile and Web Applications Engineering

---

## 1. Introduction

A **mobile application** is software installed on a smartphone from an app store (for example, an Android or iOS app). It can use device features such as the camera, push notifications and local storage.

A **web application** runs inside a browser and is opened through a URL. Nothing needs to be installed, and the same code works on phones, tablets and computers.

Both types are widely used for services like food ordering. For a college canteen, the right choice depends on who the users are, how often they use the system, and how much effort the college can spend on building and maintaining it.

## 2. Problem Analysis

The college wants students to browse the canteen menu, place orders, pay online and be told when the food is ready. Today, students probably queue at the counter, which causes:

- Long waiting times during breaks.
- Wrong or forgotten orders.
- Cash handling and billing mistakes.
- No way for students to know when their order is ready.

The system must therefore be fast, easy to use on a phone, and quick to launch across the whole campus.

## 3. Comparison of Mobile, Web and PWA Approaches

| Criteria | Mobile App (Native) | Web App | Progressive Web App (PWA) |
|---|---|---|---|
| Installation | Needed from app store | Not needed | Optional, "Add to Home Screen" |
| Platforms | Separate build for Android and iOS | One version for all devices | One version for all devices |
| Development cost and time | High | Low | Low to medium |
| Updates | Users must update the app | Instant, on the server | Instant, on the server |
| Push notifications | Fully supported | Limited | Supported (some limits on iOS) |
| Offline use | Good | Poor | Basic offline support using caching |
| Access to device features | Full | Limited | Partial |
| Reach | Only users who install it | Anyone with a link | Anyone with a link |

## 4. Selected Application Type and Justification

**Selected choice: Progressive Web Application (PWA).**

Reasons:

1. **One codebase for every student.** Students use different phones, so a single PWA avoids building and maintaining separate Android and iOS apps.
2. **No installation barrier.** Students can open a link or scan a QR code at the canteen, and can add it to their home screen if they want.
3. **Notifications are possible.** A PWA can send push notifications, which covers the "order is ready" requirement.
4. **Lower cost and quicker launch.** A college project usually has limited time and budget, and updates reach everyone immediately.
5. **Works on weak networks.** Caching lets the menu load quickly even when the campus Wi-Fi is slow.

A native mobile app would be better only if the college later needs advanced device features, but that is not required for this system.

## 5. Four Major Functionalities

1. **User login and profile** – Students sign in using their college credentials, and the system keeps their order history.
2. **Menu browsing** – Students view categories, items, prices and availability. Canteen staff can update the menu and mark items as sold out.
3. **Order placement and online payment** – Students add items to a cart, choose a pickup time and pay through UPI or another payment gateway. They receive an order number and a receipt.
4. **Order tracking and notifications** – The canteen staff update the order status (Received, Preparing, Ready), and the student gets a notification when the order is ready.

## 6. Three Development Challenges

1. **Handling rush-hour load.** Many students order at the same time during breaks. The server and database must handle peak traffic without slowing down or crashing.
2. **Secure and reliable payments.** The system must integrate a payment gateway safely and handle failed or duplicate payments correctly, so students are neither charged twice nor left without an order.
3. **Reliable notifications across devices.** Push notification support differs between browsers and operating systems (especially on iOS), so a backup such as SMS or an in-app status page may be needed.

## 7. Simple Application Workflow Diagram

```text
 ______________________________
|  1. Student opens canteen PWA |
|______________________________|
               |
 ______________|_______________
|  2. Login with college ID     |
|______________________________|
               |
 ______________|_______________
|  3. Browse menu               |
|______________________________|
               |
 ______________|_______________
|  4. Add items to cart         |
|______________________________|
               |
 ______________|_______________
|  5. Make online payment       |
|______________________________|
               |
 ______________|_______________
|  Payment successful?          |
|  NO : go back to step 4       |
|  YES: continue                |
|______________________________|
               |
 ______________|_______________
|  6. Order goes to canteen     |
|     staff                     |
|______________________________|
               |
 ______________|_______________
|  7. Staff prepare the order   |
|______________________________|
               |
 ______________|_______________
|  8. Order marked READY        |
|______________________________|
               |
 ______________|_______________
|  9. Student gets notification |
|______________________________|
               |
 ______________|_______________
| 10. Student collects food     |
|______________________________|
```

**Explanation:** The student logs in, selects items and pays. Once payment succeeds, the order reaches the canteen staff, who prepare it and mark it as ready. The system then notifies the student, who collects the food.

## 8. Conclusion

A canteen ordering system needs to reach every student quickly, work on any phone, and send alerts when food is ready. A Progressive Web Application meets all these needs with lower cost than separate native apps, and it is easier to update than traditional mobile apps. With careful handling of peak load, secure payments and notification support, a PWA is a suitable solution for the college canteen.
