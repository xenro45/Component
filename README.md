# **Component: A lightWeight ECS library.**

## **Creating logic for a tag:**

### **1. Directory Setup**
1. Create a directory on the Server or Client.
2. Within this directory, create an init.luau file.

### **2. Example Tag**
1. Create a ModuleScript in the directory.
2. Name the file an at sign (@) and the tag name following. 
    -An example name for the tag "Lava" would look like "@Lava"
**Example code:**
```luau
return function(instance: Instance)
    instance.Touched:Connect(function(otherPart: BasePart)
        if otherPart.Parent:FindFirstChild("Humanoid") then
            otherPart:FindFirstChild("Humanoid"):TakeDamage(20)
        end
    end)
end
```

## **Credits**
### **Authors**
andrewtdiz: https://github.com/andrewtdiz