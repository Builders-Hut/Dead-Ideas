# Bore

A user-facing object storage platform with labels, descriptions and extended file names for making files searchable.

## Why

Although being talked about negatively here, the inspiration largely comes from this Hackernews post: [	Gen Z Kids Don't Understand How File Systems Work](https://news.ycombinator.com/item?id=30253526).
It reminded me of how unorganized and vague my folders were. Even for people who do understand how filesystems work, they largely rely on search features to find the relevant files quickly.
When you require your 10th marksheet quickly, where do you find it, `~/Documents/acads`, `~/Backups/School` or `~/Academics/Achievements`? Wait, upon searching you realize it was there in your `~/Downloads` all along, since you haven't organized it since 2020. 
Sure, you can blame yourself for being lazy, but this is far too common to be your fault alone. Why can't we have a non-linear storage medium that doesn't require you to create a tree-like folder system to keep the files.
I soon started having a large "Dumpyard" folder and relied heavily on search to find out important documents. As it turns out, searching the file system isn't the smoothest experience.

Bore is a blob store where you simply dump your file, add labels, an optional description to make it easier to search, and whatever give it whatever long name you wish.

## How 

There is no restriction on what storage medium is used in the backend, it could be an actual object storage solution (S3, Azure blob storage, etc), or something you implemented from scratch.
The process of dumping your files should be as simple and straightforward as possible.

The key feature of bore is searchability. It is meant to be a giant pile of documents that can be retrieved within miliseconds of a search. The documents are indexed by their file names and descriptions.
With the previously stated problem, I will simply search for "Class 10 marksheet", "board result", "exam result" and the file should end up in the results.

The key is making it as magical as possible. No folders, hierarchy, permission management, inheritence. Since it's a blob store, the files wouldn't just be "documents" per se, they could be movies, photos or any general large binary files.

## Challenges Faced

Implementing a search experience that "just works". Creating a search algorithm from scratch is quite difficult, so using third party solutions is also permitted. However, fine-tuning them for specific use cases is difficult.

Typically, this is used for a single user and sharing isn't the main focus. However, implementing a sharing feature via links would require some form of checking to avoid misuse.

## Good to have features

Windows search also indexes text-based file formats contents for giving better results of searches. Similar feature could be implemented.

An extention to the above stated feature would be AI-generated descriptions of PDF files through OCR and generative text models to make it even easier to dump documents specifically.

contributed by [Kush Patel](https://github.com/libkush)
