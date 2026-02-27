# Foundations Lab Final

## Project Overview
This repository contains the final lab deliverables for the Foundations course. The project demonstrates the successful setup and configuration of a virtualized environment focused on cybersecurity best practices.

## Security Philosophy

My lab environment leverages virtualization and isolation to create a controlled "sandbox" for technical experimentation. Virtualization allows for the abstraction of physical hardware, enabling multiple operating systems to run independently on a single host. This isolation is critical; it ensures that any security risks, such as malware execution or system crashes within the lab, are contained and cannot impact the host machine's primary operating system.

### Connection to the CIA Triad

The design and maintenance of this lab environment directly align with the core principles of the CIA Triad:

*   **Confidentiality**: In this lab environment, confidentiality is enforced through logical isolation. By utilizing host-only networking and local authentication, data remains accessible only to the authorized user. As defined by the National Institute of Standards and Technology (2022), confidentiality is "preserving authorized restrictions on information access and disclosure, including means for protecting personal privacy and proprietary information" (p. 23).
*   **Integrity**: Integrity is maintained through the use of snapshots and state-tracking. These virtualization features ensure that the system remains in a known-good state and that no unauthorized or accidental modifications have occurred during testing. Maintaining this consistency is vital because integrity involves guarding against improper information modification or destruction (Cisco, 2024).
*   **Availability**: Availability is ensured by the portability and backup capabilities of virtual machines. Should the lab environment encounter an error, it can be quickly restored from a previous snapshot or re-deployed from a template, ensuring the resources remain ready for use whenever needed.

### References

Cisco. (2024). *What is the CIA triad?* https://www.cisco.com

National Institute of Standards and Technology. (2022). *Security and privacy controls for information systems and organizations* (NIST Special Publication 800-53, Rev. 5). U.S. Department of Commerce. https://doi.org
