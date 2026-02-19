# Let's get started!

    https://github.com/Azure-Samples/azure-sql-modernize-app-with-ai

# Data API builder
    https://aka.ms/salai-samples

# SQL Server 2025 Developer Edition

    https://aka.ms/sql2025dev

# Azure SQL DB Free Offer

    https://aka.ms/azuresqldbfree

# Azure SQL Dev's Corner Blog

    https://devblogs.microsoft.com/azure-sql/

# Introducing MCP Server for Oracle Database
https://www.youtube.com/watch?v=Nq6i_Ppn4cc

# Introducing MCP Server for Oracle Database
Model Context Protocol (MCP) was introduced in November 2024 by Anthropic and was met with viral adoption rates. Until MCP, large language models (LLMs) have never been able to directly interact with external data sources and APIs. Instead, the application layer was responsible for orchestrating context augmentation by using the model to enrich user questions with additional information. MCP’s explosive growth comes from the standardization of a protocol used to add context to an LLM. The absence of such a protocol meant that every tool, every API, and so on, would have to create a bespoke implementation for each platform or integration to offer the same functionality. This often led to duplicated efforts across tools and vendors, requiring developers to write custom code for each LLM provider.
    
Oracle evaluated MCP and has integrated it into our core developer tools, making the Oracle Database immediately available on any platform supporting MCP. This integration is made available via our modern command line to the Oracle Database, Oracle SQLcl.

<img width="3088" height="1272" alt="image" src="https://github.com/user-attachments/assets/d05c2905-08a4-4125-abd1-3df5850dfad2" />

# Oracle SQLcl

[Check out the key features of Oracle SQLcl:](https://social.ora.cl/60067ovU0)


#================================================================================
https://www.youtube.com/redirect?event=video_description&redir_token=QUFFLUhqbnI5MzBhZzV4NXNFY1pveVdKRk1QazlTa0ZQUXxBQ3Jtc0tsWWpjdFNKZ0VaM2xScDBrY0pzSVg5VDJVYUlPd2JxUThuVEowTzdBNGZQbXZzcDB5WVJGaEp1VGhHZThGbVpjUDB5djJPTnlPdU8yOFNKSE0zb19uLWhvY1dleGRscm5WMEdaaGROaWhNcDdIZHFRRQ&q=https%3A%2F%2Fwww.docker.com%2Fproducts%2Fdocker-desktop%2F&v=5WlyMjihfWQ

https://www.oracle.com/uk/database/free/

https://www.oracle.com/database/sqldeveloper/technologies/sqlcl/download/

https://www.oracle.com/database/sqldeveloper/technologies/sqlcl/download/

 https://claude.ai/download

https://docs.oracle.com/en/database/oracle/sql-developer-command-line/25.2/sqcug/using-oracle-sqlcl-mcp-server.html

https://github.com/bbrumm/databasestar/tree/main/sample_databases/oracle_hr




        Explanation and Demo on Model Context Protocol ( MCP) with oracle sqlcl and Claude desktop.
        
        Docker dektop - https://www.docker.com/products/docke...
        Oracle 23ai -  https://www.oracle.com/uk/database/free/
        sqlcl - https://www.oracle.com/uk/database/sq...
        Claude -  https://claude.ai/download
        SQLclmcp user guide -  https://docs.oracle.com/en/database/o...
        oracle HR sample schema  - https://github.com/bbrumm/databasesta...
        
        --Install 23ai  , Follow    • Install Oracle database using Docker - Demo  
        
          --docker
          -- pull oracle23ai image
          docker pull container-registry.oracle.com/database/free:latest
          
          --create and run a docker container 
          docker run --name oracle-23c-ai -p 1521:1521 -p 5500:5500 -e ORACLE_PWD=pwd
          -e ORACLE_CHARACTERSET=AL32UTF8 -v oracle_data:/opt/oracle/oradata 
          -d container-registry.oracle.com/database/free:latest
        
        --Create schema and run sample scripts
          
          -- use bash to create users/ change password etc  
          -- At this point, you can also use SQLDeveloper.
          docker exec -it OracleDB_23ai /bin/bash
          conn -save cline_mcp -savepwd hr/$passwword$@//localhost:1234/Database1
          
        --configure mcp server for sqlcl
          
          {
          "mcpServers": {
            "sqlcl": {
              "command": "sqlcl_bin_dir/sql",
              "args": ["-mcp"]
            }
          }  
        }
          
        -- Ask in comments if you get stuck!
        
        #mcp #oracle23ai #oraclesqlcl #sqlcl #claude #sonnet #artificialintelligence #modelcontextprotocol #oracle


