# Reportcard
Day 4 assignment 
**Program** :
pragma solidity ^0.4.17 < 0.6.12; 

contract ReportCard{
    
    string public name;
    uint public   rrn ;
    uint public batch;
    string public s1;
    string public s2;
    string public s3;
    string public s4;
    
    function ReportCard(string newName, uint newRRN, uint newBatch, string newS1, string newS2, string newS3, string newS4) public{
        
        name = newName;
        rrn = newRRN;
        batch = newBatch;
        s1 = newS1;
        s2 = newS2;
        s3 = newS3;
        s4 = newS4;
        
    }

    
    function getReportCurrentDetails() public view returns(string,uint,uint,string,string,string,string){
        return(name, rrn, batch, s1, s2, s3, s4);
    }
    
    
}

The test Deployment of the smart contract can be found @ 0xE4fc36eAbe5A4A66956574D47d793C95A54502d1 in
https://ropsten.etherscan.io/address/0xe4fc36eabe5a4a66956574d47d793c95a54502d1
