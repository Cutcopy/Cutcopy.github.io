---
layout: page
title: About
permalink: /about/
---
<div id="bookingjs">
  <script type="text/javascript" src="//ajax.googleapis.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>
  <script type="text/javascript" src="http://cdn.timekit.io/booking-js/v1/booking.min.js" defer></script>
  <script type="text/javascript">
    window.timekitBookingConfig = {
      name: 'Bryce Stradling - Web Designer',
      email: 'bryce@getvyral.com',
      apiToken: 'MZhNGg3KGEn9grx7c8oUm38N6u3x68Ul',
      calendar: 'a2004ae1-325d-4b12-8aff-4ed778ea370e',
      avatar: 'https://lh6.googleusercontent.com/-Urzx5-qR9zE/AAAAAAAAAAI/AAAAAAAADMo/G9_5UZ-LVI0/photo.jpg',
      timekitFindTime: {
        filters: {
          and: [
            {
              business_hours: { }
            },
            {
              exclude_weekend: { }
            }
          ],
          or: [
            {
              specific_time: {
                start: '00',
                end: '12'
              }
            },
            {
              specific_time: {
                start: '13',
                end: '24'
              }
            }
          ]
        }
      }
    }
  </script>
</div>

This is the base Jekyll theme. You can find out more info about customizing your Jekyll theme, as well as basic Jekyll usage documentation at [jekyllrb.com](http://jekyllrb.com/)

You can find the source code for the Jekyll new theme at: [github.com/jglovier/jekyll-new](https://github.com/jglovier/jekyll-new)

You can find the source code for Jekyll at [github.com/jekyll/jekyll](https://github.com/jekyll/jekyll)
