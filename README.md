# Simple Task List

## Description
A simple command line application to manage tasks. Users can add, view, mark and delete tasks.

## Features
- **Add new tasks:** Users can input new tasks to be tracked.
- **View All Tasks:** Users can see a list of all current tasks.
- **Mark Tasks as Complete:** Users can mark tasks as done.
- **Delete Tasks:** Users can remove tasks from the list.

## Prerequisites
-[Python](https://www.python.org/downloads/) (version 3.x)
-A code editor (e.g., Visual Studio Code) 

## Installation

1. **Clone the Repository:**
   ```bash
   git clone <https://github.com/Han137-L/s.git>
   cd SimpleTaskList

# Members
Hannan Ahmed, UGR/1910/17
Ayantu Alemu, UGR/9765/17
Eden Manasbot, UGR/1965/17
Bitanya Mesfin, UGR/5798/17
Eldana Tilaye, UGR/9955/17




# simple_task_list.py

class Task:
 def _init_(self, description):
    self.description = description
    self.completed = False

 def mark_complete(self):
    self.completed = True

 def _str_(self):
    status = "✓" if self.completed else "✗"
    return f"[{status}] {self.description}"

    
class TaskList :
 def_init_(self):
    self.tasks = []

 def add_task(self, description):
     new_task = Task(description)
     self.tasks.append(new_task)

 def view_tasks(self):
     for index, task in enumerate(self.tasks):
         print(f"{index + 1}. {task}")

 def mark_task_complete(self, index):
        if 0 <= index < len(self.tasks):
            self.tasks[index].mark_complete()
        else:
            print("Invalid task number.")

 def delete_task(self, index):
        if 0 <= index < len(self.tasks):
            del self.tasks[index]
        else:
            print("Invalid task number.")

            
         