# ACID Theorem Explained with Examples

## What is ACID?

ACID is an acronym that stands for Atomicity, Consistency, Isolation, and Durability. It represents a set of properties that guarantee reliability and integrity in database transactions.

### Atomicity

Atomicity ensures that a transaction is treated as a single, indivisible unit of work. Either all of the operations within the transaction are completed successfully, or none of them are.

**Example**: Consider a bank transfer transaction where money is debited from one account and credited to another. Atomicity ensures that if the money is debited from one account, it is also credited to the other account, and both operations are completed successfully or none of them are. There is no intermediate state where money is deducted from one account but not credited to the other.

### Consistency

Consistency ensures that a transaction brings the database from one valid state to another valid state. It preserves the integrity constraints and rules defined in the database schema.

**Example**: Suppose there is a database constraint that specifies that the sum of all withdrawals cannot exceed the account balance. Consistency ensures that after a withdrawal transaction is completed, the account balance remains consistent with this constraint. If the withdrawal would result in a balance below zero, the transaction is aborted to maintain consistency.

### Isolation

Isolation ensures that the execution of multiple transactions concurrently produces the same result as if they were executed sequentially. Each transaction is isolated from the effects of other transactions until it is completed.

**Example**: Consider two transactions: T1 transfers money from account A to account B, and T2 checks the account balance of account A. Isolation ensures that even if T1 is in progress, T2 sees a consistent state of the database. It does not see an intermediate state where the money has been debited from account A by T1 but has not yet been credited to account B.

### Durability

Durability ensures that once a transaction is committed, its changes are permanently stored in the database and are not lost, even in the event of a system failure.

**Example**: After a successful bank transfer transaction, the changes to the account balances are persisted to the database. Even if the system crashes immediately after the transaction is committed, the changes remain durable and are not lost. When the system recovers, it can restore the database to the state it was in before the crash, including the committed transaction.

## Conclusion

The ACID properties provide a framework for ensuring the reliability, integrity, and consistency of database transactions. By adhering to these principles, database systems can maintain data integrity and recoverability, even in the face of system failures or concurrent access by multiple users.
