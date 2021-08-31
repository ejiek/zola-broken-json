+++
title = "Json navigation issue"
+++

Following shortcode works fine if there is no `-` in key name.
But if there is a `-`, zola 0.14 would try to access field
pre `-` field (`bro` of `bro-ken`)

{{ broken() }}
