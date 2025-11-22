---
layout: default
title: Home
---

# 🔐 CTF Writeups

Welcome to my writeups collection! Here you'll find detailed solutions for various CTF challenges and penetration testing machines.

## 📚 Categories

- [HackTheBox](#hackthebox)
- [TryHackMe](#tryhackme)
- [CTF Competitions](#ctf)

---

## HackTheBox

{% for post in site.posts %}
  {% if post.categories contains "htb" %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
  {% endif %}
{% endfor %}

## TryHackMe

{% for post in site.posts %}
  {% if post.categories contains "thm" %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
  {% endif %}
{% endfor %}

## CTF

{% for post in site.posts %}
  {% if post.categories contains "ctf" %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
  {% endif %}
{% endfor %}
