# Base de conocimientos (reglas y hechos)
class KnowledgeBase:
    def __init__(self):
        self.rules = []
        self.facts = []
    
    def add_rule(self, rule):
        self.rules.append(rule)
    
    def add_fact(self, fact):
        self.facts.append(fact)

    def get_rules(self):
        return self.rules

    def get_facts(self):
        return self.facts
