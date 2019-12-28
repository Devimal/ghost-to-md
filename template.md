---
title: ${post.title}<% if (post.slug) { %>
slug: ${post.slug}<% } %>
template: "post"
date: "${post.publishedAt}"<% if (post.tags.length) { %>
category: ${post.tags[0]}
tags: ${post.tagArray}<% } %>
draft: <% if (post.status === 'draft') { %>true<% } else { %>false<% }%><% if (post.custom_excerpt) { %>
excerpt: ${post.custom_excerpt}<% } %>
description: ""
socialImage: "/media/image-2.jpg"
---

${post.markdown}
