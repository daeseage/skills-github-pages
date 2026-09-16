Title: Flow Charts

```mermaid
flowchart LR
    All["`**SnoCo DSA Files**`"] --> Steering["`**Steering**`"]
    Steering --> C[Financial]
    Steering --> D[Internal Elections]
    All --> HGO["`**HGOs**`"]
    HGO --> F[Case Files]
    All --> Public["`**Public Archive**
    	linked on website`"]
    Public --> H[Meeting Agendas]
    Public --> I[Resolutions]
    I --> J[Submission Form & Drafts]
    I --> K[Final - enrolled]
    I --> L[Final - did not pass]
    All --> Committee["`**Committee Files**
    	T&C manages new co-chair access. Current co-chairs delegate access to committee members. Reset co-chair access after an election.
    	All contain
  	- charter
    	- agenda/minutes
    	- committee SOPs`"]
    Committee --> N["`**Membership**
        - listwork scripts
    	- signup records`"]
    Committee --> O["`**Tech & Comms**
    	- draft posts
   	- Access inventory & credentials`"]
    Committee --> P["`**Poli Ed**
    	- Training sign ins
    	- Presentation files
    	- Book group history`"]
    Committee --> Q["`**Labor & Organizing**`"]
    Committee --> R["`**International Solidarity**`"]
    Committee --> S["`**Electoral**
    	- Endorsement docs
    	- Candidate forum docs
    	- Committee roles/membership`"]
```
<!-- Load Mermaid library from CDN -->
<script src="https://cdn.jsdelivr.net/npm/mermaid@12.0.0/dist/mermaid.min.js"></script>
<!-- Optional: Style Mermaid diagrams -->
<style>
  .mermaid {
    background-color: #f8f9fa; /* Light gray background */
    padding: 1.5rem; /* Add padding around diagrams */
    border-radius: 8px; /* Rounded corners */
    overflow-x: auto; /* Horizontal scroll for wide diagrams */
    margin: 1rem 0; /* Spacing above/below diagrams */
  }
</style>
<!-- Initialize Mermaid and render diagrams -->
<script>
  // Wait for the page to fully load
  document.addEventListener('DOMContentLoaded', function() {
    // Find all Markdown code blocks with class "language-mermaid"
    const mermaidCodeBlocks = document.querySelectorAll('pre code.language-mermaid');
 
    // Convert each code block into a Mermaid diagram
    mermaidCodeBlocks.forEach(block => {
      // Create a new div for Mermaid to render into
      const mermaidDiv = document.createElement('div');
      mermaidDiv.className = 'mermaid'; // Match the CSS class above
      mermaidDiv.textContent = block.textContent; // Copy diagram code
 
      // Replace the original code block with the Mermaid div
      block.parentNode.replaceChild(mermaidDiv, block);
    });
 
    // Initialize Mermaid with default settings
    mermaid.initialize({
      startOnLoad: true, // Render diagrams when Mermaid loads
      theme: 'default', // Use default theme (options: default, dark, forest, neutral)
      logLevel: 3 // Suppress non-critical logs (0 = debug, 3 = error)
    });
  });
</script>
