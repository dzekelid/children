---
name: VMWare
x-slug: vmware
description: At VMware, we believe that software has the power to unlock new opportunities
  for people and our planet. We look beyond the barriers of compromise to engineer
  new ways to make technologies work together seamlessly. Our software forms a digital
  foundation that powers the apps, services and experiences that are transforming
  the world.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Children
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/children/master/_listings/vmware/apis.md
specificationVersion: "0.14"
apis:
- name: vRealize Operations 6 - Add Child Resource to a Resource
  x-api-slug: apiresourcesosresourceidrelationshipschildren-post
  description: "This operation adds a child resource to a resource.  \n\nAPI documentation
    states that POST is additive while PUT is destructive (i.e. overwites existing
    relationships).\n\nJSON body includes an array of child objects to add.  \n\nThe
    call does not provide a lot of detail for failure, but it seems\nthat if you have
    an invalid UUID for a child or the child is already related\nthen it will fail
    with 400.\n\n204 is a successful call."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/children/master/_listings/vmware/apiresourcesosresourceidrelationshipschildren-post-openapi.md
- name: vRealize Operations 6 - Add Child Resource to a Resource
  x-api-slug: apiresourcesosresourceidrelationshipschildren-post
  description: "This operation adds a child resource to a resource.  \n\nAPI documentation
    states that POST is additive while PUT is destructive (i.e. overwites existing
    relationships).\n\nJSON body includes an array of child objects to add.  \n\nThe
    call does not provide a lot of detail for failure, but it seems\nthat if you have
    an invalid UUID for a child or the child is already related\nthen it will fail
    with 400.\n\n204 is a successful call."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/children/master/_listings/vmware/apiresourcesosresourceidrelationshipschildren-post-openapi.md
x-common:
- type: x-blog
  url: https://blogs.vmware.com/
- type: x-blog-rss
  url: http://blogs.vmware.com/all-vmware-blogs/wprss
- type: x-github
  url: https://github.com/VMware
- type: x-twitter
  url: https://twitter.com/VMware
- type: x-website
  url: http://vmware.com
- type: x-api-gallery
  url: http://visage.cloud.api.gallery.streamdata.io
- type: x-api-stack
  url: http://vmware.stack.network
- type: x-curated-source
  url: https://blogs.vmware.com/vcloud/2015/12/vmware-vcloud-air-network-compliance-spotlight-hipaa.html
- type: x-website
  url: https://www.vmware.com
- type: x-branding
  url: https://www.vmware.com/brand/our-brand.html
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---