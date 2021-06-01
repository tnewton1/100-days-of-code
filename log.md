# 100 Days Of Code - Log

### Day 0: May 26, 2021

**Today's Progress**: Worked on Chapter 9 "Classes" pages 171, 172, and exercise 9-6.

**Thoughts:** I struggled a bit with the exercise, but I've learned that building up a code library helps. I was able to re-use exercise 9-4 as a base and to add the additional class and attributes. I also had to reach back and use a loop and a list. I haven't used these lately. 

**Link to work:** 
1. [Commit 6c55707](https://github.com/tnewton1/python-crash-course/commit/6c55707c01792880ff6555d09467b2494a107651)
2. [Commit 6ef1f81](https://github.com/tnewton1/python-crash-course/commit/6ef1f816ed629579ecf8cb183bd99895aa53a0cf)

### Day 1: May 27, 2020

**Today's Progress**: Worked more on Chapter 9 "Classes", excercise 9-7.

**Thoughts:** I'm wondering if this will get easier. I found myself having to reference back a little bit and struggled a bit to get some of my code to work. Eventually, though, I did have a moment where it hit me on what I needed to do and then I got it working.

**Link to work:**
[Commit 2793189](https://github.com/tnewton1/python-crash-course/commit/27931898b27bb645c82f30d8172791786e1adb46)

### Day 2: May 28, 2020

**Today's Progress**: Worked more on Chapter 9 "Classes", excercise 9-8.

**Thoughts:** This was a particularly hard challenge for me. I had to look a few things up in order to get it to work. Turns out, I really messed it up. I guess I was extra tired which didn't help. While Exercise 9-7 is _kind of_ correct, it actually isn't. I should have created an empty list for permissions. For example, this is just wrong:

```
class Admin(User):
    def __init__(self, first_name, last_name):
        super().__init__(first_name, last_name)
        self.privileges = ['can add post', 'can delete post', 'can ban user', 'can edit post', 'can delete user', 'can change username']

    def show_privileges(self):
        print("Assigned privileges: ")
        for privileges in self.privileges:
            print(f"\n· {privileges.title()}")
```

It should be:

```
class Admin(User):
    def __init__(self, first_name, last_name):
        super().__init__(first_name, last_name)
        self.privileges = []

    def show_privileges(self):
        print("Assigned privileges: ")
        for privileges in self.privileges:
            print(f"\n· {privileges.title()}")
```

And then you would define the privileges by creating a list later on. Oh well. Lesson learned! 

**Link to work:**
[Commit fb5963d](https://github.com/tnewton1/python-crash-course/commit/fb5963d5ba757a042975987b0ef9232619772b33)

### Day 3: May 29, 2021

**Today's Progress**: Worked more on Chapter 9. Completed exercise 9-9, and part of Importing Classes, pages 174-176.

**Thoughts:** I am noticing I am starting to notice the patterns in the code and where I can reuse stuff. I did not find exercise 9-9 too challenging. It was pretty easy to figure out. Importing classes is a great topic to be on as I find it particularly helpful to be organized in code and this helps me out. I was noticing that some of these files were getting long and a bit chaotic. Breaking them up helps!

**Link to work:**
1. [Commit ad072d7](https://github.com/tnewton1/python-crash-course/commit/ad072d7d59dd11d95dd770d8d66fe8f70db03c16)
2. [Commit 3f9233b](https://github.com/tnewton1/python-crash-course/commit/3f9233b46af602b61f1f985aaeb49ecde577bb4f)

### Day 4: May 30, 2021

**Today's Progress**: Simple day. Worked on importing multiple classes, page 177

**Thoughts:** I took an easy day today. I'm promising myself to do more tomorrow. This was just importing multiple classes. It was fairly simple and not too hard.

**Link to work:**
1. [Commit 786e248](https://github.com/tnewton1/python-crash-course/commit/786e248932f2c2b6007371e02abfd20092a5fab3)

### Day 5: May 31, 2021

**Today's Progress**: Another simple day. Pages 177-180, exercises 9-10 and 9-11.

**Thoughts:** It was another easy day. Just working on some simple exercises and redoing some exercises with new skills.

**Link to work:**
1. [Commit 584c54d](https://github.com/tnewton1/python-crash-course/commit/584c54d09275f332ac64ff0794173be8d9240bff)
