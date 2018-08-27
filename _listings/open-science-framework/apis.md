---
name: Open Science Framework
x-slug: open-science-framework
description: OSF provides free and open source project management support for researchers
  across the entire research lifecycle. As a collaboration tool, OSF helps researchers
  work on projects privately with a limited number of collaborators and make parts
  of their projects public, or make all the project publicly accessible for broader
  dissemination. As a workflow system, OSF enables connections to the many services
  researchers already use to streamline their process and increase efficiency. As
  a flexible repository, it can store and archive research data, protocols, and materials.
image: ""
x-kinRank: "7"
x-alexaRank: "0"
tags: Children
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/children/master/_listings/open-science-framework/apis.md
specificationVersion: "0.14"
apis:
- name: Open Science Framework - List all child nodes
  x-api-slug: nodesnode-idchildren-get
  description: |-
    A paginated list of the next level child nodes for the given node. The returned nodes are sorted by their `date_modified`, with the most recently updated child nodes appearing first.

    The list will include child nodes that are public, as well as child nodes that are private, if the authenticated user has permission to view them.
    #### Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of up to 10 child nodes. If the given node has zero child nodes, the `data` key will contain an empty array. Each resource in the array is a separate node object and contains the full representation of the child node, meaning additional requests to the child node's detail view are not necessary.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

    This request should never return an error.
    #### Filtering
    You can optionally request that the response only include nodes that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/nodes/ezcuj/children/?filter[title]=reproducibility.

    Nodes may be filtered by their `id`, `title`, `category`, `description`, `public`, `tags`, `date_created`, `date_modified`, `root`, `parent`, `preprint`, and `contributors`.

    Most fields are string fields and will be filtered using simple substring matching. Public and preprint are boolean fields, and can be filtered using truthy values, such as **true**, **false**, **0** or **1**. Note that quoting true or false in the query will cause the match to fail.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/children/master/_listings/open-science-framework/nodesnode-idchildren-get-openapi.md
- name: Open Science Framework - Create a child node
  x-api-slug: nodesnode-idchildren-post
  description: |-
    Creates a new child node.

    Note: Creating a child node via this endpoint will function the same as creating a node via the node list endpoint, but the child node will have the given node set as its parent.
    #### Permissions
    Only write contributors may create children nodes.
    #### Required
    Required fields for creating a node include:

    &nbsp;&nbsp;&nbsp;&nbsp`title`

    &nbsp;&nbsp;&nbsp;&nbsp`category`

    Note: nodes default to **private** unless the `public` field is explicitly set to **true** in the request payload.
    #### Returns
    Returns a JSON object with a `data` key containing the representation of the created node, if the request is successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/children/master/_listings/open-science-framework/nodesnode-idchildren-post-openapi.md
- name: Open Science Framework - List all child registrations
  x-api-slug: registrationsregistration-idchildren-get
  description: |-
    A paginated list of children of a registration.

    The list consists of the next level child registrations for the given registration. The returned registrations are sorted by their `date_modified`, with the most recently updated child registrations appearing first.

    The list will include child registrations that are public, as well as child registrations that are private, if the authenticated user has permission to view them.
    #### Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of up to 10 child registrations. If the given registration has zero child registrations, the `data` key will contain an empty array. Each resource in the array is a separate registration object and contains the full representation of the child registration.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

    #### Filtering
    You can optionally request that the response only include registrations that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wucr8/children/?filter[title]=reproducibility.

    Registrations may be filtered by their `id`, `title`, `category`, `description`, `public`, `tags`, `date_created`, `date_modified`, `root`, `parent`, and `contributors`.

    Most fields are string fields and will be filtered using simple substring matching. Public is a boolean field, and can be filtered using truthy values, such as **true**, **false**, **0** or **1**. Note that quoting true or false in the query will cause the match to fail.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/children/master/_listings/open-science-framework/registrationsregistration-idchildren-get-openapi.md
x-common:
- type: x-website
  url: https://cos.io
- type: x-api-gallery
  url: http://open.fintech.api.gallery.streamdata.io
- type: x-api-stack
  url: http://open.science.framework.stack.network
- type: x-github
  url: https://github.com/OSFramework
- type: x-twitter
  url: https://twitter.com/OSFramework
- type: x-website
  url: http://osf.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---