```mermaid
erDiagram
    PROJECT {
        string Name
        string Description
        string Concept
        PM[] AssignedPMs
        Vendor[] ApprovedVendors
        Team[] Teams
        blob SRS
        string[] Roles         
    }
    MODULE {
        string Name
        ModuleType Type
        string Summary 
        string Details
        string ThemeUI
        string PM
    }
    SERVICE {
        string Name        
        string Summary
        string Description 
        ServiceType Type 
        string API_Interface 
        Dependency[] Dependencies
        string Deployment_Bundle
        PM PM
    }
    LIBRARY {
        string Name
        string Description
        string CodeLanguage
        string Version
        string UML
        string BPML
        string PM
        string CodeConvention
    }
    CLASS {
        string Name
        Interface[] Interfaces
        string Description
        string UX
        string UI
        UserStory Story
        PM AssignedPM
        Vendor Vendor
        ClassType Type 
        Interface[] DependencyInterfaces 
        string[] MocksStubs
    }
    JOB {
        JobType Type 
        Class[] Classes
        Library[] Libraries
        DateTime Deadline
        float Budget 
        PM PM
    }
    PHASE {
        string Name
        DateTime Deadline 
    }
    TASK {
        string Name
        Class Class 
        Library Library
        Vendor Vendor 
        DateTime StartTime 
        DateTime EndTime 
        TaskType Type 
        Policy Policy        
    }
    JOBTEMPLATE {
        string Name
        PhaseTemplate PhaseTemplate
    }
    PHASETEMPLATE {
        string Name
        int TimeAllocation
        TaskTemplate TaskTemplate
    }
    TASKTEMPLATE {
        string Name
        string Type
    }
```

 * ModuleType (DB, Repository, UI)
 * ServiceType (DB, Doc Repository, Business Logic, UI) 
 * Dependencies (DB, Doc Repository) 
 * ClassType (Main, Integration Test, Load Test, Performance Test) 
 * VendorType (UX, UI, coder, QA, QM)
 * JobType (UML, BPML, Use Cases, Project Docs, Classes, Services, Modules, UI, UX, Theme)
 TaskType (Manual, Automation) 
 PolicyType (Read/Write ?) 