---
title: Contentstack Web Destination
id: 66ccaa142d6b2d223bb1ebda
---

> info "This destination sends data in device-mode"
> This destination transmits data from the browser directly to Contentstack on the client-side. Contentstack supports both device-mode and cloud-mode destinations. For more about the Cloud-mode destination, see [Contentstack Cloud Destination](/docs/connections/destinations/catalog/actions-contentstack).

[Contentstack](https://www.contentstack.com/?utm_source=segment&utm_medium=docs&utm_campaign=partners){:target="_blank”} is a headless CMS that allows you to build digital experiences using a modular approach. This integration lets you sync data from Segment to your Contentstack Personalize project, enabling dynamic and personalized content delivery.

This destination is maintained by Contentstack. For any issues with the destination, [contact their Support team](https://www.contentstack.com/customers/support){:target="_blank”}.

## Prerequisites

- a Contentstack account with Personalize enabled
- a Contentstack Personalize project created in your Contentstack organization

## Before you begin

- **Contentstack Personalize Project**: Create a Contentstack Personalize project within your organization and link your Contentstack stack to enable variant functionality.
- **Attributes & Audiences**: Define attributes and create audiences based on those attributes within your Contentstack Personalize project.
- **Events**: Define and create the events that you want to track and sync with your Contentstack Personalize project.

## Getting started

1. From your workspace's [Destination catalog page](https://app.segment.com/goto-my-workspace/destinations/catalog){:target="_blank”} search for "Contentstack Web".
2. Select Contentstack Web and click **Add Destination**.
3. Select an existing Source to connect to Contentstack Web.
4. Go to the Contentstack account and find the following parameters to input as settings in the Segment destiantion settings:
  - **Personalize Project ID**: Enter the unique ID of your Contentstack Personalize project.
  - **Personalize Edge API Base URL**: Enter the base URL of your Contentstack Personalize API. You can find this URL in the Contentstack documentation.

{% include components/actions-fields.html %}

## Send events to Segment

Start sending the payload of events to Segment using track or identify calls. This will not only send events to Segment but will forward the selected values to Contentstack Personalization. Ensure your event payloads align with the mapping configuration you created for the Contentstack destination in Segment.

## Receive personalized content

Based on your events/payloads, your Contentstack Personalize project should now start receiving events for understanding the users associated with your mapped values.

The event names and properties you use must match those defined in your Contentstack Personalize project. For advanced customization and to further enhance your personalized experience, explore Contentstack Personalize in [Contentstack's Documentation](https://www.contentstack.com/docs/personalize){:target="_blank”}.
