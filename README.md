# Innovatex
BREX Quality of life changes
#include <stdio.h>
#include <string.h>

#define MAX_USERS 100
#define SUPPORT_TICKETS 50

typedef struct {
    char name[50];
    int business_age_months;
    float monthly_revenue;
    int risk_score; // 0 = safe, 1 = medium, 2 = high risk
    int account_frozen;
} SMBUser;

typedef struct {
    int ticket_id;
    char issue;
    int resolved;
} SupportTicket;

SMBUser users[MAX_USERS];
SupportTicket tickets[SUPPORT_TICKETS];
