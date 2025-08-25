# Friday AI Malware Analysis Tool - Sample Questions Guide

## 📋 Overview
This guide provides comprehensive sample questions you can ask Friday in speak mode. The AI system intelligently routes questions between Gemini and Perplexity for optimal responses.

---

## 🔍 **LOCAL DATA COMMANDS** (No AI quota required)

### View Available Data
```
show fields for 75dddb
read a1b2c3 scans
show f4e5d6 contacted_urls
read 123abc detection_names
```

### Quick Data Access
```
read <MD5> contacted_urls
read <MD5> contacted_domains  
read <MD5> contacted_ips
read <MD5> scans
read <MD5> detection_names
read <MD5> file_type
read <MD5> size
read <MD5> first_submission_date
read <MD5> last_analysis_date
read <MD5> reputation
read <MD5> crowdsourced_yara_results
read <MD5> sandbox_verdicts
read <MD5> capabilities
read <MD5> behavior_summary
```

---

## 🤖 **AI-POWERED QUESTIONS** (Smart routing with auto-failover)

### 📊 **Sample Classification & Overview**
```
What type of malware is this sample?
Is this file malicious or benign?
What's the verdict for sample 75dddb?
Classify this malware family
What detection engines flagged this sample?
How many antivirus engines detected this as malware?
Give me a summary of the analysis results
What's the risk level of this sample?
```

### 🔍 **Behavioral Analysis**
```
What malicious behaviors does this sample exhibit?
Analyze the behavioral patterns of this malware
What capabilities does this malware have?
Describe the malware's execution techniques
What system changes does this malware make?
How does this sample evade detection?
What persistence mechanisms does it use?
Analyze the malware's communication patterns
What files does this malware create or modify?
Describe the network activity of this sample
```

### 🌐 **Network & Communication Analysis**
```
What URLs does this malware contact?
Analyze the network indicators for this sample
What domains does this malware communicate with?
Are there any suspicious IP addresses contacted?
What's the command and control infrastructure?
Analyze the HTTP requests made by this malware
What external resources does it download?
Describe the network communication patterns
Are there any known malicious URLs contacted?
What ports does this malware use for communication?
```

### 🛡️ **Detection & Evasion Analysis**
```
Which antivirus engines detected this sample?
What detection names were assigned to this malware?
How does this malware attempt to evade detection?
What anti-analysis techniques are used?
Are there any false positive indicators?
How reliable are the detections for this sample?
What YARA rules matched this sample?
Analyze the detection confidence levels
Are there any sandbox evasion techniques?
What obfuscation methods are employed?
```

### 🔗 **Threat Intelligence & Attribution**
```
What malware family does this belong to?
Are there any APT campaign connections?
What threat actors might be behind this?
Compare this sample to known threat families
What are the TTPs (Tactics, Techniques, Procedures)?
Is this related to any known campaigns?
What's the geographical targeting of this malware?
Analyze potential attribution indicators
What similar samples have been seen before?
Is this part of a larger attack campaign?
```

### ⚠️ **Risk Assessment & Impact**
```
What's the potential impact of this malware?
How dangerous is this sample to enterprise networks?
What systems would this malware target?
Assess the risk level for financial institutions
What data could this malware steal?
How would this affect critical infrastructure?
What's the business impact of this threat?
Rate the severity of this malware sample
What industries does this malware typically target?
How quickly should this threat be addressed?
```

### 🔧 **Technical Deep Dive**
```
Analyze the PE header information
What packing or compression is used?
Examine the import/export functions
What cryptographic algorithms are implemented?
Analyze the code structure and complexity
What development tools were likely used?
Examine the file metadata and timestamps
What are the technical indicators of compromise?
Analyze the malware's encryption methods
Describe the payload delivery mechanism
```

### 📈 **Comparative Analysis**
```
Compare this sample to other malware in the dataset
How does this relate to recent threat trends?
What makes this sample unique or common?
Compare detection rates across different engines
How does this sample's behavior differ from benign files?
What's unusual about this malware's characteristics?
Compare this to previous versions of the same family
How sophisticated is this compared to typical malware?
What evolution patterns can be seen in this family?
Compare the evasion techniques to industry standards
```

### 🔮 **Predictive & Strategic Analysis**
```
What future variants might emerge from this family?
How might this malware evolve over time?
What defensive measures should be implemented?
Predict the likely attack scenarios for this malware
What indicators should security teams monitor?
How can organizations prepare for similar threats?
What's the expected lifespan of this threat?
Recommend detection and prevention strategies
What security controls would be most effective?
How should incident response be prioritized?
```

---

## 🎯 **FORCE-ROUTING COMMANDS**

### Use Gemini AI Specifically
```
@gemini What are the main characteristics of this malware?
@gemini Analyze the behavioral patterns
@gemini Provide a detailed technical analysis
```

### Use Perplexity AI Specifically  
```
@perplexity What threat intelligence is available for this sample?
@perplexity Compare this to current threat landscapes
@perplexity Research the latest trends in this malware family
```

---

## 🛠️ **EXAMPLE CONVERSATION FLOWS**

### Quick Analysis Workflow
```
1. "What type of malware is sample 75dddb?"
2. "What behaviors does it exhibit?"
3. "What networks does it contact?"
4. "How dangerous is this threat?"
5. "What should I do to defend against it?"
```

### Deep Investigation Workflow
```
1. "Analyze all behavioral patterns for sample a1b2c3"
2. "What evasion techniques does it use?"
3. "Compare this to known APT families"
4. "What's the attribution likelihood?"
5. "Provide comprehensive remediation recommendations"
```

### Threat Hunting Workflow
```
1. "What IOCs should I extract from this sample?"
2. "What network signatures can I create?"
3. "What similar samples should I look for?"
4. "How can I hunt for this family in my environment?"
```

---

## 💡 **TIPS FOR BETTER RESPONSES**

### ✅ **Best Practices**
- Be specific about what aspect you want analyzed
- Use natural language - the AI understands context
- Ask follow-up questions to dive deeper
- Combine multiple data points in your questions
- Reference specific MD5 hashes when possible

### ⚡ **Quick Commands**
- Type "stop" during speech to interrupt TTS
- Use shorter MD5 prefixes (e.g., "75dddb" instead of full hash)
- Ask "show fields for <MD5>" to see available data fields
- Use "exit" to quit the speak mode

### 🎯 **Query Types That Work Well**
- **Analytical**: "Analyze the..." "What patterns..."  
- **Comparative**: "Compare this to..." "How does this differ..."
- **Explanatory**: "Explain why..." "How does this work..."
- **Predictive**: "What might happen..." "How could this evolve..."
- **Actionable**: "What should I do..." "How can I defend..."

---

## 📊 **DATA FIELDS REFERENCE**

Common JSON fields you can explore:
- `scans` - Detection results from all engines
- `contacted_urls` - URLs contacted by malware
- `contacted_domains` - Domains contacted  
- `contacted_ips` - IP addresses contacted
- `detection_names` - Names assigned by AV engines
- `capabilities` - Malware capabilities
- `behavior_summary` - Behavioral analysis summary
- `file_type` - File type information
- `size` - File size
- `first_submission_date` - When first seen
- `last_analysis_date` - Most recent analysis
- `reputation` - Reputation score
- `crowdsourced_yara_results` - YARA rule matches
- `sandbox_verdicts` - Sandbox analysis results

Use "show fields for <MD5>" to see all available fields for any specific sample.

---

This comprehensive guide gives you the full range of questions you can ask Friday's AI system for malware analysis!

Note :AI features are in beta stage and also it give the data of vt json data for that sample 
