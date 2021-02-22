
---
wp_id: 204
wp_post_status: "publish" 
title: "The Cryptic Problem of Encryption"
date: 2013-06-06T13:26:46+05:00
date_modified: 2013-07-11T12:54:49+05:00
date_published: 2013-06-06T13:26:46+05:00
primary_category: "Uncategorized"
categories: ['Uncategorized'] 
tags: ['data', 'security', 'tools', 'collaboration']
seo_title: "the cryptic problem of encryption"
seo_meta_description: ""
summary: ""
featured_image_url: "no image"
slug: "the-cryptic-problem-of-encryption"
url: "https://www.inciter.io/the-cryptic-problem-of-encryption/"
authors: CRC
---

#Content

<span style="color: #ff9900;">_by Sarah McCruden_</span>
So you’ve compiled some raw data for your next big report, or, you’ve come across a few clients’ records that have errors that need to be addressed. If you need to share these tasks with a coworker, email is often the most convenient method for sharing: just attach and send! Sounds simple. But, have you ever wondered just how the email makes its way to the recipient—and whether it’s really safe on its journey there?
According to Leo Notenboom, a personal computer and software industry expert, concerns about email interception may be exaggerated: “It is possible to sniff and eavesdrop on email conversations. It's also not particularly easy, unless you're on an open WiFi connection.” Yet, he goes on to say that, “by default, the contents of email is not encrypted or obscured in any way. As it travels from your computer to your mail server to my mail server and finally to my PC, it's stored in formats that are easily read by anyone who has access and cares to do so” (<a href="http://ask-leo.com/just_how_secure_is_email_anyway.html" target="_blank" title="How Secure is Email Anyway?">Notenboom, 2013</a>).
I must say that, as a database analyst who compiles datasets for clients and coworkers on a daily basis, this is enough to make me nervous. The fact is that research is a field where collection of data isn’t just a small part of the job—it’s the foundation of it. Obtaining and, inevitably, transferring and storing private information is integral to most research efforts, so security should be one of our top concerns.&nbsp;So how are we to protect our data if we need or prefer to use email? The answer is data encryption. However, its implementation is not as simple as you might think. Encrypting your data essentially means scrambling it so that interception by anyone aside from the intended recipient would yield an unreadable document. Sounds perfect, right?
Well, unfortunately, as Notenboom points out, “the problem here is that encryption schemes for email are generally not as interoperable as we'd like… while some solutions are free, often they involve third-party software and periodic fees.”&nbsp;He goes on to suggest a few free options that will encrypt a file in ZIP format using software that password protects it, but the issue with this (and with the “Encrypt with Password” option available on any Microsoft Office document), is that you must then communicate the password to the recipient, which is all too often done via… you guessed it… email. The password must be communicated through a different channel, but practically speaking, do you have time to call or text a recipient any time you want to send a document so that they can safely get the password and read the contents?
Because, like me, you probably do not, a better option would be to get your company on-board with using public key cryptography. Public key cryptography uses public-private key pairs, as opposed to password encryption, which uses one common password that the sender and the recipient must share. With public key cryptography, it’s as if you’ve sent many copies of a padlock (your public key) to those who need to send you private data, while keeping the one key that fits the padlock (your private key) safely stored on your computer alone. By using your digital signature in a message to your recipient, their computer can store your unique public key (“lock”) and digital certificate as part of your email contact card. When they need to send you sensitive data—or anything really—they can put your lock on the outgoing email, and your computer will automatically use its private key to decode it, without you ever having to enter any sort of passcode. Only once a public key is paired with the unique corresponding private key will the contents be decrypted and readable.
Keep in mind that to get a digital signature and your public key “lock,” you’ll need a digital ID—and that is a paid service. It’s not terribly expensive, but it does pose some limitations on when you can use public key cryptography: if you’ve got the paid service, anyone with whom you’ve shared your public key can send encrypted data TO you, but they cannot receive encrypted data FROM you without having paying for a digital ID themselves. So if your whole company is on-board you can safely send and receive encrypted documents to your coworkers, but when it comes time to send a report to an outside associate, you’re out of luck if they haven’t paid for a digital ID.
So what’s the safest solution? I’m a proponent of using public key encryption wherever you can—you can at least make sure that incoming private data is protected. Obviously, you can’t supply digital IDs to everyone you interact with, and in those cases password encryption will do in a pinch. What do you think is the best way to deal with this problem: work towards getting others onboard with digital IDs? Use password encryption and some sort of system to communicate them? Or just never use email for sensitive data period? We’re eager to hear what you think!
&nbsp;
Source: &nbsp;Leo A. Notenboom. _Ask Leo: Just How Secure Is Email, Anyway?_ Puget Sound Software, LLC, 2003-2013. Web. 3 June 2013.

